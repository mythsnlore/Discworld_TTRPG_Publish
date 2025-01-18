---
Important: false
PartyHasMet: false
Race:
---
<% tp.file.title %>
<% await tp.file.move("/World/Characters/" + tp.file.title) %>

<%*
const hasTitle = !tp.file.title.startsWith("NewNPC");
let title;
if (!hasTitle){
	title = await tp.system.prompt("Enter NPC Name");
} else {
	title = tp.file.title;
}
_%>

Name of dude: <% tp.file.cursor() %>
Cool dude?
Race: `INPUT[inlineListSuggester(option(apple), option(banana), option(lemon)):Race]`
Item: 


Stats
Notes