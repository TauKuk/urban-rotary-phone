# ✨ Lumin

> A community-powered search engine for **learning anything** – where results are ranked by **helpfulness, novelty, and quality**, not by ads or SEO.

---

## 🔍 What is this?

Curated Skill Search is a learning-focused discovery engine.

You type in a **skill you want to learn** – anything from *sourdough bread* to *Rust programming* to *game theory* – and the platform returns a curated list of:

- 📝 Articles & guides  
- 🎥 Videos & courses  
- 🛠 Tools & apps  
- 📚 Books & long-form resources  

All **submitted and voted on by the community**, ranked by how *helpful*, *novel*, and *well-explained* they are for learning that skill.

The goal: make it easy to find **hidden gems** and *actually good* learning resources, instead of whatever happens to be most marketed on traditional search engines.

---

## 🎯 Motivation

Traditional search engines and feeds are optimized for:

- Clicks, ads, and engagement  
- SEO tricks and generic content  
- Mainstream, already-popular results  

They are **not** optimized for:

- Deep, hands-on learning  
- Finding niche or high-signal resources  
- Surfacing *novel* approaches and formats  

We want a place you go to **specifically when you want to learn something**, where:

- Every result is **intentional** (submitted by someone who found it useful)  
- The community votes on **usefulness**, **clarity**, and **originality**  
- You can filter by **format**, **difficulty**, and **time investment**

---

## 🧩 Core Concepts

- **Skill-centric search**  
  The main entry point is: *“What do you want to learn?”*. Results are organized around skills/topics, not generic keywords.

- **User-submitted resources**  
  Anyone can submit links or uploads: articles, YouTube videos, MOOCs, tools, GitHub repos, etc.

- **Voting on usefulness & novelty**  
  Users upvote based on:
  - *How helpful was this for learning?*
  - *How clear/accessible is it?*
  - *Is it novel/interesting or just the same generic stuff?*

- **Multi-format support**  
  A skill might be best learned through:
  - a long-form blog post  
  - a 20-min video  
  - an interactive tool  
  - a GitHub template  
  Users can filter by these formats.

- **Signals over popularity**  
  Ranking is based on:
  - Helpfulness votes
  - Novelty/uniqueness signals
  - Engagement from people who actually **studied** with it  
  Not just total views or clickbait.

- **Learning-focused, not entertainment**  
  The platform is explicitly **for learning**. Not memes, not doomscrolling, not random browsing.

---

## ✨ Planned Features (MVP)

- 🔎 **Search**
  - Search by skill, topic, or sub-skill (e.g. “intro to options trading”, “espresso extraction”, “React hooks”).

- 📥 **Submit resources**
  - Submit a URL or upload content.
  - Tag the skill(s), level (beginner/intermediate/advanced), and format (article / video / course / tool / etc.).

- 👍 **Voting & reviews**
  - Upvote based on helpfulness & novelty.
  - Optional short review: *“Helped me understand X when others didn’t”*.

- 🏷 **Filters**
  - Filter by:
    - Format (video, article, interactive, app…)
    - Level (beginner / intermediate / advanced)
    - Time length (e.g. < 15 min, 1–2 hours, multi-week course)

- 🧑‍💻 **User profiles (basic)**
  - See what someone has liked or recommended.
  - Minimal reputation/karma system tied to quality of shared resources.

- 🧠 **Skill pages**
  - Each skill has its own page:
    - Top community-voted resources
    - New & rising resources
    - Possibly curated “starter packs” later.

---

## 🏗️ Architecture (draft)

> This section is intentionally high-level and can be updated once the stack is locked in.

- **Frontend**
  - STACK: TO BE DECIDED
  - Main components:
    - Search bar + results
    - Skill pages
    - Submission form
    - Filters + sorting

- **Backend**
  - STACK: TO BE DECIDED
  - Endpoints for:
    - Searching resources
    - Submitting resources
    - Voting / reviews
    - Managing skills & tags

- **Database**
  - Postgres (Or a graph database? TBD) for:
    - Users
    - Skills
    - Resources
    - Votes / reviews
    - Tags & formats

- **Search layer**
  - Simple version: DB-backed search with indices
  - Later: dedicated search engine (e.g. Meilisearch / Elasticsearch / OpenSearch)

---

## 🚀 Getting Started (development)

### Prerequisites

- PostgreSQL (or your chosen DB)

### 1. Clone the repo

```bash
git clone git@github.com:DziugasD/urban-rotary-phone.git
cd urban-rotary-phone
```