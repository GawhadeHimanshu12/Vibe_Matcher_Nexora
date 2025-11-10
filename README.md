# Vibe Matcher – AI-Powered Fashion Recommendation - Assignment For Nexora
---

## Overview

**Vibe Matcher** is a prototype recommendation system that matches user *vibe* queries (e.g., “energetic urban chic”) with fashion products using **OpenAI’s embedding model** `text-embedding-ada-002`.  
It demonstrates how semantic similarity can go beyond keyword search — helping users discover products that *feel right* instead of just matching words.

This project was built as part of a technical assessment for **Nexora**, focusing on AI-driven semantic understanding and intelligent product discovery.

---

## Why AI at Nexora?

AI at Nexora is about creating more intuitive, human-like shopping experiences. Instead of relying on rigid keyword filters, AI can capture the *vibe*, tone, and context behind a customer’s search.  
By embedding both product descriptions and user intent into high-dimensional semantic space, Nexora can deliver smarter, context-aware recommendations that increase engagement, conversion, and satisfaction.

---

## Features

- Uses **OpenAI’s `text-embedding-ada-002`** model for real embeddings  
- Computes **cosine similarity** to identify top-3 vibe-matched products  
- Supports both **default and user-input queries** via an interactive menu  
- Caches embeddings locally to reduce API calls and improve performance  
- Logs latency, similarity metrics, and exports results to CSV  
- Handles **edge cases** gracefully (e.g., nonsense or minimal queries)  

---

## How It Works

1. **Data Preparation:**  
   A small dataset (8 fashion items) is created with descriptive text, categories, prices, and vibe tags.

2. **Embedding Generation:**  
   Product texts (name + description + vibes) are embedded using OpenAI’s `text-embedding-ada-002` model.

3. **Similarity Search:**  
   User queries are embedded, and cosine similarity is computed against all product embeddings to find the top matches.

4. **Evaluation:**  
   The notebook tests three default queries, measures similarity scores, latency, and logs metrics to CSV.




