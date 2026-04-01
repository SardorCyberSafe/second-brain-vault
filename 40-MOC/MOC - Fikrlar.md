---
title: "MOC - Fikrlar"
created: {{date}}
tags:
  - moc
topic: thoughts
---

# 🗺️ MOC — Fikrlar

## 📌 Umumiy Ko'rinish
Xom fikrlardan pishiq bilimgacha bo'lgan yo'l.

## 💭 Fleeting Notes
```dataview
TABLE created, status
FROM "10-Fleeting"
WHERE status = "raw"
SORT created DESC
LIMIT 10
```

## 🧠 Permanent Notes
```dataview
TABLE type, created, updated
FROM "30-Permanent"
SORT updated DESC
LIMIT 10
```

## 📊 Statistikalar
- **Jami Fleeting:** `=length(rows(filter(file.inlinks, (f) => startswith(f.path, "10-Fleeting"))))`
- **Jami Permanent:** `=length(rows(filter(file.inlinks, (f) => startswith(f.path, "30-Permanent"))))`

## 🔄 Konversiya Jarayoni
1. `00-Inbox` → Tezkor capture
2. `10-Fleeting` → Xom fikr
3. `30-Permanent` → Pishiq bilim (bog'langan)

## 🔗 Bog'liq
- [[MOC - Asosiy]]
- [[Templates/Fleeting Note]]
- [[Templates/Permanent Note]]

---
#moc #thoughts #pkm
