
```dataview
table Status, file.mtime as "Last Change", file.folder as "Loc",   
from ""
where Status = "~complete" or Status = "incomplete" or Status = "progress"
sort Status asc, file.folder asc
```



<iframe src="https://github.com/Anirudh025/ParagonHero_Obsidian" width=700 height = 800></iframe>
