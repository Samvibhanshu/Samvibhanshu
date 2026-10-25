### Hi, I'm Samridhi 👋

B.Tech Computer Science (Business Systems) at **VIT Vellore**, graduating 2027. I build backend systems in Java and clean, usable frontends, and I work on applied ML research: inventor on **six patent applications** (five published) and author of **three papers submitted to IEEE Access**.

---

#### Backend and systems (Java)

| Project | What it is | Evidence |
|---|---|---|
| [**order-service**](https://github.com/Samvibhanshu/order-service) | E-commerce order backend: place, pay, ship, cancel over a JSON HTTP API. No overselling under concurrency (per-SKU locks taken in sorted order, so no deadlock), idempotency keys so a retried payment never charges twice, and a single order state machine. | 30 tests, including 64 threads racing for the last 50 units |
| [**mini-sqs**](https://github.com/Samvibhanshu/mini-sqs) | A message queue with Amazon SQS semantics: visibility timeouts, receipt handles, dead-letter queues and redrive, FIFO groups with deduplication, long polling, and a worker pool with exponential backoff. | 26 tests, including 600 randomized operation sequences and multi-threaded producers and consumers |
| [**route-planner**](https://github.com/Samvibhanshu/route-planner) | Delivery routing: BFS, Dijkstra, A\* and bidirectional Dijkstra on a city road network, plus delivery rounds through many stops (Held–Karp exact, nearest neighbour + 2-opt). | 19 tests against Floyd–Warshall and brute-force permutations; A\* settles 2.2× fewer nodes |

#### Other projects

| Project | What it is | Stack |
|---|---|---|
| [**Trust Decay Prediction**](https://github.com/Samvibhanshu/Trust-Decay-Prediction) | Predicts which IT assets are losing trust, from audit events in a temporal knowledge graph, and ranks them for audit with explanations. Dashboard plus JSON API. Auditing the model's top 10% each day finds High/Critical decay 47% of the time vs 31% for random picks (simulated enterprise). | Python, scikit-learn, networkx, Flask · 68 tests |
| [**Autonomous Wildfire Prediction**](https://github.com/Samvibhanshu/Autonomous-Wildfire-Prediction-Response-System) | Wildfire-risk ensemble on the UCI Forest Fires data with resource orchestration and a live dashboard. The models are constrained so hotter, drier weather can never lower the predicted risk, and the README reports measured accuracy next to the projected figures. | Python, scikit-learn, Flask, SQLite · 71 tests |
| [**Notes App**](https://github.com/Samvibhanshu/Notes-App) | Create, edit, search, copy and delete notes, persisted in the browser. Pure Redux reducers with persistence in a store subscriber; corrupted storage cannot crash it. Deployed on Vercel. | React 19, TypeScript, Redux Toolkit, Vite, Tailwind · 13 tests |
| [**Found-It**](https://github.com/Samvibhanshu/Found-It) | Campus lost-and-found web app. Team project; I wrote most of the commits. | Next.js, React, Tailwind |

#### Patents

Patent applications filed through the VIT IPR Cell, each taken from idea to working prototype:

* **Autonomous wildfire risk prediction** with resource-orchestrated response (published) · [code](https://github.com/Samvibhanshu/Autonomous-Wildfire-Prediction-Response-System)
* **Information-system trust-decay prediction** on temporal knowledge graphs for continuous audit intelligence (published) · [code](https://github.com/Samvibhanshu/Trust-Decay-Prediction)
* **Hybrid edge-AI mine tremor detection** with distributed IoT sensor nodes and multi-node consensus (published)
* **Provenance-aware organic sentiment estimation** that separates genuine opinion from reposts, bots and AI rewrites (published)
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

**Languages:** Java, Python, TypeScript, JavaScript, C/C++, SQL, R &nbsp;·&nbsp; **Web:** React, Next.js, Node.js, Express, Tailwind CSS, Redux Toolkit &nbsp;·&nbsp; **AI/ML:** scikit-learn, LangChain, RAG, Oracle Cloud Infrastructure

**Certified:** Oracle Cloud Infrastructure 2025 Generative AI Professional

📫 [Portfolio](https://samvibhanshu.github.io) · [Email](mailto:samridhivibhanshu305@gmail.com)
