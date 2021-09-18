---
tags: ⚙️
aliases: 
cssclass:
---
%% This note requires the data view plugin %%
```dataview
list 
from "" AND !"CRM" AND !"Ancestry" AND !"Journal"
where file.day
sort file.day desc
```

---
list from "" AND !"Journal" where type != null AND file.day sort file.day desc