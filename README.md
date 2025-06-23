# 🧠 Adaptive Sharding System for E-Commerce Products

This project demonstrates an intelligent **sharding and load balancing** mechanism over Amazon product data. It simulates a real-time product categorization, query routing, and load monitoring system — enabling dynamic scaling and rebalancing of data shards based on discount levels, category popularity, and access patterns.

---

## 📦 Dataset

The project uses a cleaned version of `amazon.csv` which includes:
- Product categories
- Ratings and review counts
- Actual and discounted prices
- Discount percentages

---

## 🚀 Features

- ✅ Cleans and preprocesses Amazon product data
- 🧠 Extracts top-level categories
- 🔀 Computes **adaptive shard IDs** based on:
  - Category
  - Rating activity level (low/high)
  - Discount level (low/high)
- 📈 Generates `shard_metadata.json` for insights
- 🔍 Uses **semantic search (Sentence Transformers)** for fuzzy user input
- 🔁 Logs user queries and shard access with latency
- 📊 Performs monitoring of access load, latency, and P95 metrics
- ⚠️ Detects **hotspots** and underutilized shards
- 🔄 Rebalances overloaded shards
- 📤 Exports final stats to human-readable JSON

---
