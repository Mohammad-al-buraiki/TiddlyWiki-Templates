📁 How to Add the “Contents” Tab to Your Sidebar
To create a dynamic Contents tab that automatically shows linked pages by tag, follow these steps:

🧱 Create a New Tiddler with the Following Settings:
Tiddler Title:
Contents (or any name you want — this is what will appear in the sidebar)

Tag:
$:/tags/SideBar

Body (Tiddler Content):

html
Copy
Edit
<div class="tc-table-of-contents">
<<toc-selective-expandable 'Contents' sort[title]>>
</div>
Field Name:
list-before

Field Value:
$:/core/ui/SideBar/Open

✅ Once added and saved, your sidebar will show a new tab named Contents, and any tiddler tagged with Contents will show up listed underneath — including expandable sub-items based on their tags.
