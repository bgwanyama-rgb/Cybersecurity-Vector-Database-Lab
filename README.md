# Cybersecurity-Vector-Database-Lab

This lab teaches you how to build and query a **local cybersecurity vector database** using:

- Python
- ChromaDB
- Sentence Transformers
- MITRE ATT&CK techniques
- OpenAI API

You will learn how to:

- Build embeddings
- Store vectors in a persistent database
- Perform semantic search
- Integrate with AI tools like VS Code Copilot, Cursor and OpenAI

---

# Lab Steps

Follow the steps in order.

1. [Install Prerequisites](docs/01_prerequisites.md)
2. [Open the Project in VS Code](docs/02_open_project.md)
3. [Create Python Environment](docs/03_setup_environment.md)
4. [Install Dependencies](docs/04_install_dependencies.md)
5. [Build the Vector Database](docs/05_build_vector_database.md)
6. [Query the Database](docs/06_query_vector_database.md)
7. [Use with AI Tools](docs/07_use_with_ai_tools.md)
8. [Recommended Workflow](docs/08_workflow.md)
9. [Troubleshooting](docs/09_troubleshooting.md)

---

# Project Structure

```
scripts/
    ingest.py
    query.py

data/
vector_store/
requirements.txt
```

---

# Expected Output

When the system works correctly you should see:

```
Persistent cybersecurity memory created.
```

and queries will return relevant MITRE techniques.

---

# Learning Outcome

By completing this lab you will understand:

- Vector embeddings
- Semantic similarity search
- Retrieval Augmented Generation (RAG)
- Local AI knowledge bases
