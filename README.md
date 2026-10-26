### Hi, I'm Samridhi 👋

B.Tech in Computer Science and Engineering (specialization in Business Studies) at **VIT Vellore**, CGPA **9.81**, graduating 2027.
I build backend systems in Java, and I turn research ideas into working, tested prototypes: **six patent applications**
(five published) and **three papers** submitted to IEEE Access.

Looking for **software engineering internships**. Portfolio, with a page for every project: **[samvibhanshu.github.io](https://samvibhanshu.github.io)**

---

#### Systems in Java

No frameworks or dependencies, so every line can be read and explained. Each has CI running its tests, and each README
says what it does not do.

| Project | What it is | What backs it up |
|---|---|---|
| [**order-service**](https://github.com/Samvibhanshu/order-service) · [page](https://samvibhanshu.github.io/projects/order-service.html) | E-commerce order backend over a JSON HTTP API. Never oversells (per-SKU locks in sorted order, so no deadlock), never charges twice (idempotency keys), and survives crashes: a write-ahead log with checksums and group commit, replayed on start. | 44 tests, incl. 64 threads racing for the last 50 units and a server killed with `kill -9` mid-traffic, four times, losing nothing it acknowledged |
| [**order-service-aws**](https://github.com/Samvibhanshu/order-service-aws) · [page](https://samvibhanshu.github.io/projects/order-service-aws.html) | The same service on **AWS Lambda, API Gateway and DynamoDB**, every rule enforced by conditional writes and transactions. AWS request signing (SigV4) written from scratch and checked against botocore. SAM template. | 18 tests against DynamoDB's API, incl. 32 requests racing for 20 units |
| [**mini-sqs**](https://github.com/Samvibhanshu/mini-sqs) · [page](https://samvibhanshu.github.io/projects/mini-sqs.html) | A message queue with Amazon SQS semantics (visibility timeouts, dead-letter queues, FIFO groups, long polling), also served over HTTP in **SQS's own wire protocol**, so the official AWS SDK works against it. | 39 tests; the AWS SDK for Python passes 27 checks against it in CI |
| [**agentic-bug-repair**](https://github.com/Samvibhanshu/agentic-bug-repair) · [page](https://samvibhanshu.github.io/projects/agentic-bug-repair.html) | Takes a Java repository with failing tests and tries to fix it: measures which methods each test runs, ranks where the bug probably is, tries small patches in a sandbox, and only proposes a pull request that passes every test on a clean checkout. | 154 tests; on 20 seeded bugs it correctly fixes 8 (up from 4), and ranks the buggy method first for 11 of 20 (held-out MRR 0.36 → 0.61) |
| [**route-planner**](https://github.com/Samvibhanshu/route-planner) · [page](https://samvibhanshu.github.io/projects/route-planner.html) | Delivery routing: BFS, Dijkstra, A\* and bidirectional Dijkstra, plus delivery rounds (Held–Karp exact, nearest neighbour + 2-opt). | 19 tests against Floyd–Warshall and brute force; A\* settles 2.2× fewer nodes |

#### Research prototypes

Working code for the patent applications below, each with tests and an honest results section.

| Project | What it is | Stack |
|---|---|---|
| [**Opinion lineage**](https://github.com/Samvibhanshu/opinion-lineage) | Organic sentiment from social media: tracks which posts copy which, weights by independence, corrects a retracted source without re-running models (16 ms vs 511 ms for 50,000 records). | Python, NumPy, scikit-learn · 27 tests |
| [**Trust Decay Prediction**](https://github.com/Samvibhanshu/Trust-Decay-Prediction) | Forecasts which IT assets are losing trust from audit events in a temporal knowledge graph; the daily top-10% audit list finds high-risk assets 47% of the time vs 31% at random (simulated). | Python, scikit-learn, NetworkX, Flask · 68 tests |
| [**Risk-Constrained Emergency Control**](https://github.com/Samvibhanshu/Risk-Constrained-Emergency-Control-System) | Screens an emergency ventilation action before a small reversible test: 0.8% false-safe rate, 92.9% of harmful actions caught (simulated). [Browser demo](https://samvibhanshu.github.io/demos/emergency-control/). | Python, scikit-learn · 37 tests |
| [**Wildfire Prediction**](https://github.com/Samvibhanshu/Autonomous-Wildfire-Prediction-Response-System) | Wildfire-risk ensemble on UCI Forest Fires with resource orchestration; constrained so hotter, drier weather can never lower the risk. | Python, scikit-learn, Flask · 71 tests |
| **Hybrid Fall Detection** | Random Forest on SisFall and an edge-AI wearable (ESP32 + MPU6050) that confirms falls and alerts caregivers through Blynk IoT. Code not public yet. | Python, C++, ESP32 |

#### Web apps

| Project | What it is | Stack |
|---|---|---|
| [**Notes App**](https://github.com/Samvibhanshu/Notes-App) | Notes persisted in the browser; pure Redux reducers, and corrupted storage cannot crash it. Deployed on Vercel. | React 19, TypeScript, Redux Toolkit · 13 tests |
| [**Found-It**](https://github.com/Samvibhanshu/Found-It) | Campus lost-and-found front end with image upload. Team project. | Next.js, React, Tailwind |

#### Patents and papers

Six patent applications through the VIT IPR Cell (five published): wildfire risk prediction (202641083188), mine tremor
detection (202641075003), opinion lineage (202641115708), IS trust-decay prediction (202641108535), risk-constrained
emergency control, and predictive railway collision avoidance (filed). Three papers submitted to *IEEE Access* (2026),
under review. [Details](https://samvibhanshu.github.io/research.html).

#### Experience

* **Board Member (Core Lead), CSI-VIT** (Sep 2025 – present): leading the development, design, operations and outreach teams.
* **Full Stack Developer, CSI-VIT** (Aug 2024 – present): React and Tailwind work on the Laser Tag event site (1,000+ visitors) and GitHub data visualisation for the team.
* **Programme Representative, VIT** (Jul 2024 – present): liaison for 200+ students on academic concerns and curriculum feedback.

#### Tools

**Languages:** Java, Python, JavaScript, TypeScript, SQL, C, C++, R  
**Backend and cloud:** concurrency, REST APIs, write-ahead logging, AWS Lambda, API Gateway, DynamoDB, SAM, Flask  
**Front end:** React, Next.js, Redux, Tailwind CSS  
**ML and data:** scikit-learn, pandas, NumPy, NetworkX, RAG  
**Testing and CI:** pytest, Vitest, my own Java test kits, randomized and crash tests, GitHub Actions  
**Certified:** OCI 2025 Generative AI Professional · OCI 2025 AI Foundations Associate

📫 [Portfolio](https://samvibhanshu.github.io) · [LinkedIn](https://www.linkedin.com/in/samridhi-vibhanshu-09771b27a/) · [Email](mailto:samridhivibhanshu305@gmail.com)
