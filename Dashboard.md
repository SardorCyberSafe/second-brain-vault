---
title: Dashboard
created: {{date}}
tags:
  - dashboard
---

# 🧠 Ikkinchi Miya — Dashboard

---

## 📥 Inbox
```dataview
TABLE created, tags
FROM "00-Inbox"
SORT created DESC
```

---

## 🚀 Aktiv Loyihalar
```dataview
TABLE status, priority, deadline
FROM "50-Projects/Active"
WHERE status = "active"
SORT priority ASC
```

---

## 📖 O'qilayotgan
```dataview
TABLE author, type, rating, status
FROM "20-Literature"
WHERE status = "reading"
SORT created DESC
```

---

## 🗺️ MOC lar
```dataview
TABLE topic, created
FROM "40-MOC"
SORT created DESC
```

---

## 📅 Bugungi Daily Note
```dataview
TABLE mood, energy
FROM "Daily"
WHERE day = date(today)
```

---

## 🧠 Flashcard Review
```dataview
TABLE topic, difficulty, created
FROM #flashcard
SORT created DESC
LIMIT 10
```

---

## 📊 Haftalik Review
```dataview
TABLE week, created
FROM "Reviews"
WHERE contains(tags, "weekly")
SORT created DESC
LIMIT 4
```

---

## 🔗 Tezkor Havolalar
- [[MOC - Asosiy]]
- [[MOC - O'rganish]]
- [[MOC - Loyihalar]]

---
#dashboard
