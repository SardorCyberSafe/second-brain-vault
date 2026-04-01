---
title: "MOC - Loyihalar"
created: {{date}}
tags:
  - moc
topic: projects
---

# 🗺️ MOC — Loyihalar

## 📌 Umumiy Ko'rinish
Barcha aktiv va tugallangan loyihalar markazi.

## 🚀 Aktiv Loyihalar
```dataview
TABLE status, priority, deadline
FROM "50-Projects/Active"
WHERE status = "active"
SORT priority ASC
```

## ✅ Tugallangan Loyihalar
```dataview
TABLE status, priority, deadline
FROM "50-Projects/Completed"
WHERE status = "completed"
SORT deadline DESC
```

## 📊 Loyiha Holatlari
| Holat | Soni |
|-------|------|
| Active | `=length(filter(file.tasks, (t) => !t.completed))` |
| Completed | `=length(filter(file.tasks, (t) => t.completed))` |

## 🔗 Bog'liq
- [[MOC - Asosiy]]
- [[Templates/Project]]
- [[Templates/Weekly Review]]

---
#moc #projects
