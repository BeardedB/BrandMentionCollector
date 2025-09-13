# Mention Collector — Facebook Webhook + Polling Connector

This repository contains a Facebook webhook receiver (FastAPI) and a polling fallback to collect Page posts and comments, normalize them and index into OpenSearch.

**Purpose:** quickly spin up a dev-friendly mention collector for Facebook Pages (feed, comments, mentions) with webhook verification and a polling fallback. Suitable as the foundation to extend connectors (X, TikTok, LinkedIn, News).

---

## Quick start (local dev)

1. **Create repo and paste files**  
   Create a new GitHub repo and add these files.

2. **Copy `.env.example` → `.env`**  
   Fill values (see below). Do NOT commit `.env`.

3. **Run with Docker Compose (easy)**  
   Install Docker & Docker Compose, then:
   ```bash
   docker compose up --build
