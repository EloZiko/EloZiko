# Zakaria El Ouahidi

Student at **Harvard University**, in the AI & Robotics Lab, advised by Dr. Wang.  
Before that: MEng in Computer Science at **CentraleSupélec**, Paris-Saclay University.

Currently working on **world models**, **spatial reasoning for VLMs** and **flow matching**.

<br>

**ML/DL:** Python · PyTorch · Scikit-learn · Pandas  
**LLMs:** HF Transformers · LangChain · OpenAI API · RAG  
**Infra:** Slurm · GPU clusters · Git · LaTeX

<br>

## Projects

<details>
<summary><b>Predicting oxygen dependency in newborns with a diaphragmatic hernia</b> · co-first author, paper in writing</summary>

<br>

Congenital Diaphragmatic Hernia (CDH) is a rare disease, about 1 in 3,000 foetuses: a hole in the diaphragm lets the stomach, liver and other organs move into the thorax and compress the heart and lungs.
Doctors can predict survival quite well from ultrasound and MRI, but not whether the baby will need long-term oxygen. That information matters a lot for parents.

With AP-HP and the Kremlin-Bicêtre hospital (France's reference center for CDH), we built a model that predicts, **before birth**, oxygen dependency at day 28 of life.

- 4 routine prenatal markers, chosen on clinical grounds
- 6 classifiers compared (logistic regression, random forest, XGBoost, HistGradientBoosting, CatBoost, TabPFN), tuned with nested cross-validation
- trained on 50 fetuses (Paris-Saclay), validated on an **independent cohort of 98 fetuses from Leuven, Belgium**
- best model: CatBoost, **external AUC 0.827**

The data stays confidential, the code is open: [CDH-oxygen-d28-prediction](https://github.com/EloZiko/CDH-oxygen-d28-prediction)

</details>

<details>
<summary><b>MCQ generator for the start-up Cleaverlearn</b> · LLM pipeline</summary>

<br>

![Cleaverlearn_gif](https://github.com/user-attachments/assets/981a499a-5264-4948-b550-2d1c1e020cee)

Generates multiple-choice quizzes from educational content (Wikipedia, Markdown).
Modular NLP pipeline, with Pydantic validation at each stage.

- **LLM (OpenAI GPT):** prompt engineering for concept extraction and Q&A generation
- **Semantic clustering:** sentence-transformers + cosine similarity to group similar concepts
- **Scraping:** BeautifulSoup with a JSON caching/indexing system

Pipeline: `ConceptExtractor` → `ConceptClusterCombiner` → `QuestionAnswerGenerator` → `DistractorGenerator` → `QCMCleaner`

</details>

<details>
<summary><b>Terraria x Minecraft x 2048</b> · a game in Pygame</summary>

<br>

Explore a procedurally generated 2D world, mine numbered tiles (2 → 2048), go home and play 2048 with them. Your score unlocks better pickaxes, which unlock harder blocks.

Dirt (no req.) → Stone (16+ tile) → Obsidian (64+ tile) → Deep resources (256+ tile)

- MVC architecture, Pygame-CE at 60 FPS
- custom physics: gravity, parabolic jumps (V₀ = 564, max jump = 2.3 blocks), collisions
- viewport culling for large backgrounds
- two worlds (overworld ↔ house) with seamless transitions
- player animation state machine and inventory

</details>

<details>
<summary><b>Cheer Up! CentraleSupélec website</b> · HTML / CSS / JS</summary>

<br>

With the Cheer Up! association, I built the team's website with Anaël Anzala and helped organize solidarity projects, including weekly visits to Gustave Roussy Hospital to support children with cancer.

→ [cheerup-cs.fr](https://www.cheerup-cs.fr/)

</details>
