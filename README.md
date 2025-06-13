# 🧠 TDS Virtual Teaching Assistant

A FastAPI-based Virtual Teaching Assistant (TA) that answers student questions from the **Tools in Data Science (TDS)** course offered by **IIT Madras Online Degree Program**.

This assistant uses:
- 🧾 Course content (Markdown files)
- 💬 Discourse forum discussions (`all_discourse.json`)
- 🔎 Retrieval-Augmented Generation (RAG)
- 🧠 Embeddings + Vector DB (ChromaDB)
- 🌐 Hosted on [Render](https://render.com/)

---
## 🧩 Discourse & Course Content Scraping

The `/scraping/` folder contains:
- `course_scraping.py` – scrapes course pages into markdown
- `discourse_scraping.py` – fetches Discourse posts by date range
- `discourse_posts.json` – scraped discourse output
- `metadata.json`, `auth.json` – metadata of course content + credentials

These scripts demonstrate the ability to generate structured datasets dynamically, as required for the bonus criteria.

## 🚀 Deployed App

**API Endpoint:**  
👉 [`https://tds-virtual-ta-cr2c.onrender.com/query`](https://tds-virtual-ta-cr2c.onrender.com/query)

### Sample cURL Test:

```bash
curl https://tds-virtual-ta-cr2c.onrender.com/query \
  -H "Content-Type: application/json" \
  -d '{"question": "What is Prompt Engineering?"}'
