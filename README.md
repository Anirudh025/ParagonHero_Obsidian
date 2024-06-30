
```dataview
table Status, file.mtime as "Last Change", file.folder as "Loc"  
from ""
where Status = "~complete" or Status = "incomplete" or Status = "progress"
sort by Status asc, file.folder


<iframe src="https://github.com/Anirudh025/ParagonHero_Obsidian" width=700 height = 800></iframe>
