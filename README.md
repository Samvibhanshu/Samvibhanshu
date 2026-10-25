### Hi, I'm Samridhi 👋

Computer science (business systems) at **VIT Vellore**, graduating 2027. I build backend systems in Java and the web apps on top of them, and I turn research ideas into working, tested prototypes: **six patent applications** (five published) and **three papers** submitted to IEEE Access.

Looking for **software engineering internships**. Portfolio: **[samvibhanshu.github.io](https://samvibhanshu.github.io)**

---

#### Systems in Java

Plain Java 17, no frameworks or dependencies, so every line can be read and explained. Each one has CI running its tests.

| Project | What it is | What backs it up |
|---|---|---|
| [**agentic-bug-repair**](https://github.com/Samvibhanshu/agentic-bug-repair) | Takes a Java repository with failing tests and tries to fix it: indexes the code as a call graph, ranks where the bug probably is, tries small patches in an isolated sandbox, and only proposes a pull request whose diff passes every test on a clean checkout. GitHub webhook and a live dashboard. | 148 tests. Benchmark on 20 seeded bugs, reported honestly: 4 repaired without a model, and why the rest were not |
| [**order-service**](https://github.com/Samvibhanshu/order-service) | E-commerce order backend: place, pay, ship, cancel over a JSON HTTP API. No overselling under concurrency (per-SKU locks taken in sorted order, so no deadlock), idempotency keys so a retried payment never charges twice, one order state machine. | 30 tests, including 64 threads racing for the last 50 units |
| [**mini-sqs**](https://github.com/Samvibhanshu/mini-sqs) | A message queue with Amazon SQS semantics: visibility timeouts, receipt handles, dead-letter queues and redrive, FIFO groups with deduplication, long polling, and a worker pool with exponential backoff. | 26 tests, including 600 random operation sequences that check no message is lost or duplicated |
| [**route-planner**](https://github.com/Samvibhanshu/route-planner) | Delivery routing: BFS, Dijkstra, A\* and bidirectional Dijkstra on a city road network, plus delivery rounds through many stops (Held–Karp exact, nearest neighbour + 2-opt). | 19 tests against Floyd–Warshall and brute force; A\* settles 2.2× fewer nodes |

#### Research prototypes

Working code for the patent applications below, each with its tests and an honest results section (what the method beats, and what it does not).

| Project | What it is | Stack |
|---|---|---|
| [**Opinion lineage**](https://github.com/Samvibhanshu/opinion-lineage) | Measures organic sentiment by tracking which posts copy, paraphrase or AI-rewrite which; a retracted source re-weights only its descendants, with no model re-runs. Includes a lineage-aware RAG layer that cites independent posts and abstains when evidence is thin. | Python, NumPy, scikit-learn, networkx · 27 tests |
| [**Trust Decay Prediction**](https://github.com/Samvibhanshu/Trust-Decay-Prediction) | Predicts which IT assets are losing trust from audit events in a temporal knowledge graph and ranks them for audit with explanations. Auditing the model's top 10% each day finds High/Critical decay 47% of the time vs 31% for random picks (simulated enterprise). Dashboard and JSON API. | Python, scikit-learn, networkx, Flask · 68 tests |
| [**Autonomous Wildfire Prediction**](https://github.com/Samvibhanshu/Autonomous-Wildfire-Prediction-Response-System) | Wildfire-risk ensemble on the UCI Forest Fires data with resource orchestration and a live dashboard. The models are constrained so hotter, drier weather can never lower the predicted risk. | Python, scikit-learn, Flask, SQLite · 71 tests |

#### Web apps

| Project | What it is | Stack |
|---|---|---|
| [**Notes App**](https://github.com/Samvibhanshu/Notes-App) | Create, edit, search, copy and delete notes, persisted in the browser. Pure Redux reducers; corrupted storage cannot crash it. Deployed on Vercel. | React 19, TypeScript, Redux Toolkit, Vite, Tailwind · 13 tests |
| [**Found-It**](https://github.com/Samvibhanshu/Found-It) | Campus lost-and-found front end with image upload. Team project; I wrote most of the commits. | Next.js, React, Tailwind |

#### Patents

Patent applications filed through the VIT IPR Cell:

* **Autonomous wildfire risk prediction** with resource-orchestrated response (published) · [code](https://github.com/Samvibhanshu/Autonomous-Wildfire-Prediction-Response-System)
* **Information-system trust-decay prediction** on temporal knowledge graphs for continuous audit intelligence (published) · [code](https://github.com/Samvibhanshu/Trust-Decay-Prediction)
* **Provenance-aware organic sentiment estimation** that separates genuine opinion from reposts, bots and AI rewrites (published) · [code](https://github.com/Samvibhanshu/opinion-lineage)
* **Hybrid edge-AI mine tremor detection** with distributed IoT sensor nodes and multi-node consensus (published)
* **Risk-constrained emergency control** using reversible micro-interventions (published)
* **Predictive railway collision avoidance** (filed)

#### Papers

Submitted to *IEEE Access* (2026):

* Physics-Shielded Conformal Learning for Network-Aware Railway Collision-Risk Assessment Under Degraded Observations
* Forecasting Information-System Trust Decay on Temporal Knowledge Graphs With Delayed-Feedback Conformal Audit Selection
* Confidence-Weighted Opinion Lineage for Organic Sentiment Estimation Under Synthetic and Coordinated Amplification

#### Experience

* **Full Stack Developer, CSI-VIT** (Aug 2024 – present): React and Tailwind work on the Laser Tag event site (1,000+ visitors) and GitHub data visualisation for the team.
* **Core Committee Member, CSI-VIT** (Apr 2024 – present): event logistics for 1,000+ participants.
* **Programme Representative, VIT** (Jul 2024 – present): liaison for 200+ students on academic concerns and curriculum feedback.

#### Tools

**Languages:** Java, Python, TypeScript, JavaScript, C/C++, SQL, R  
**Backend:** concurrency (java.util.concurrent), REST/JSON APIs, Node.js, Express, Flask  
**Front end:** React, Next.js, Redux Toolkit, Tailwind CSS, Vite  
**ML and data:** scikit-learn, pandas, NumPy, networkx, LangChain, RAG  
**Testing and CI:** JUnit-style test kits, pytest, Vitest, GitHub Actions  
**Certified:** Oracle Cloud Infrastructure 2025 Generative AI Professional

📫 [Portfolio](https://samvibhanshu.github.io) · [LinkedIn](https://www.linkedin.com/in/samridhi-vibhanshu-09771b27a/) · [Email](mailto:samridhivibhanshu305@gmail.com)
