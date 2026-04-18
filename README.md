# 🎬 Product Dissection for YouTube

> **Platform:** YouTube | **Type:** Schema Design & ER Diagram Case Study

---

## 📌 Project Overview

This project is a detailed product dissection of **YouTube** — the world's
largest video-sharing platform with 2.7 billion monthly active users.

The goal was to:
- Research YouTube's core features and user interactions
- Identify real-world problems YouTube solves
- Design a relational database schema for the platform
- Create an Entity-Relationship (ER) Diagram

---

## 📂 Files in this Repository

| File | Description |
|------|-------------|
| `YouTube_Product_Dissection_Final.docx` | Complete project document |
| `er_diagram.png` | ER Diagram created on dbdiagram.io |

---

## 🧩 Schema Design — Entities

| Entity | Purpose |
|--------|---------|
| Users | Stores all user/creator account data |
| Videos | Core content entity |
| Comments | User comments with reply support |
| Likes | Like/Dislike reactions on videos |
| Subscriptions | User-to-user subscription relationships |
| Tags | Keywords for video categorization |
| VideoTags | Junction table for Video ↔ Tag (Many:Many) |

---

## 🔗 Relationships

- User → Video **(1:Many)**
- Video → Comment **(1:Many)**
- User → Comment **(1:Many)**
- Comment → Comment **(Self-referential)**
- User → Like **(1:Many)**
- User ↔ User via Subscriptions **(Many:Many)**
- Video ↔ Tag via VideoTags **(Many:Many)**


---

## 🛠️ Tools Used

- **Schema Design:** dbdiagram.io
- **Database:** PostgreSQL
- **Document:** Microsoft Word (.docx)

---

## 👤 Author

**Pawan Ajay Prasad**
