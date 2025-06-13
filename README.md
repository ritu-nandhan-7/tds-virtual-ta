# 🧠 TDS Virtual Teaching Assistant

A FastAPI-based Virtual Teaching Assistant (TA) that answers student questions from the **Tools in Data Science (TDS)** course offered by **IIT Madras Online Degree Program**.

This assistant uses:
- 🧾 Course content (Markdown files)
- 💬 Discourse forum discussions (`all_discourse.json`)
- 🔎 Retrieval-Augmented Generation (RAG)
- 🧠 Embeddings + Vector DB (ChromaDB)
- 🌐 Hosted on [Render](https://render.com/)

---

## 🚀 Deployed App

**API Endpoint:**  
👉 [`https://tds-virtual-ta-cr2c.onrender.com/query`](https://tds-virtual-ta-cr2c.onrender.com/query)

### Sample cURL Test:

```bash
curl https://tds-virtual-ta-cr2c.onrender.com/query \
  -H "Content-Type: application/json" \
  -d '{"question": "What is Prompt Engineering?"}'
