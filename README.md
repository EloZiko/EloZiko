# Hello, I'm Zakaria El Ouahidi👋
I'm a CS MEng student at Centrale Supélec, Paris-Saclay University


## 🔧 Technologies & Tools
![Python](https://img.shields.io/badge/Python-yellow)
![Java](https://img.shields.io/badge/Java-orange)
![HTML](https://shields.io/badge/HTML-%E2%98%85%E2%98%85%E2%98%85%E2%98%85%E2%98%85-f06529?logo=html5&logoColor=white&labelColor=f06529)
![ML](https://img.shields.io/badge/Machine_learning-stronggreen)
![DL](https://img.shields.io/badge/Deep_learning-green)
![Stats](https://img.shields.io/badge/Statistics-blue)


## My projects 

### Building a model to predict neonatal bronchopulmonary dysplasia  
Congenital Diaphragmatic Hernia is a rare disease affecting about 1 in 3,000 foetuses, characterized by a hole in the diaphragm that allows the stomach, liver and other organs to move into the thorax and compress the heart and lungs. Depending on the severity and timing of the condition, this can cause lung and heart development issues and, in the most serious cases, can be life-threatening.

Specialists use ultrasound and MRI to assess the disease and potentially schedule an operation to mitigate the impact on the lungs. They are usually confident about survival rates, but are less able to predict whether the foetus will require long-term respiratory support or only a period of close surveillance. Since this information is crucial for parents in their decision-making about continuing pregnancy, AP-HP and the Kremlin-Bicêtre hospital lab, France’s reference center for the disease, asked us to train models on their data to see if prediction capability could be improved.

This project is currently underway and managed by a team of five.

Due to confidentiality I am unable to disclose any code or dataset regarding this mission.


### Developed a QCM generator for the start-up Cleaverlearn

![Cleaverlearn_gif](https://github.com/user-attachments/assets/981a499a-5264-4948-b550-2d1c1e020cee)

Automatic multiple-choice question generator from educational content (Wikipedia, Markdown).

#### 🎯 Architecture:

Modular NLP pipeline to transform raw text into structured quizzes with Pydantic validation at each stage.

#### Key Technologies:

- LLM (OpenAI GPT): Prompt engineering for concept extraction and Q&A generation
- Semantic clustering: sentence-transformers + cosine similarity to group similar concepts
- Smart scraping: BeautifulSoup with JSON caching/indexing system
- Composable pipelines: Modular architecture with detailed logging

#### Main pipelines:

- ConceptExtractor: Identifies key pedagogical concepts
- ConceptClusterCombiner: Groups by semantic similarity
- QuestionAnswerGenerator: Creates relevant questions
- DistractorGenerator: Generates plausible wrong answers
- QCMCleaner: Final JSON validation and formatting

### Terraria x Minecraft x 2048 game

A hybrid game combining sandbox exploration with puzzle mechanics. Mine numbered blocks in a procedurally generated world, then play 2048 with collected tiles to unlock better pickaxes.

#### Concept
Explore a 2D world, mine numbered tiles (2→2048) from terrain blocks, play 2048 in your house, and unlock colored pickaxes based on your score to access harder materials.

Progression: Dirt (no req.) → Stone (16+ tile) → Obsidian (64+ tile) → Deep resources (256+ tile)

#### Technical Architecture
Modular MVC Design with optimized rendering and custom physics.

#### Key Technologies:
- Game Engine: Pygame-CE for 60 FPS performance
- Physics: Custom gravity simulation (V₀ = 564, max jump = 2.3 blocks)
- Rendering: Viewport culling + .convert() optimization for large backgrounds
- State Management: Dual-world system with seamless transitions
- Player System: Inventory management, physics (parabolic jumps, collision), animation state machine
- Background Renderer: Procedural generation, optimized culling, dual-world (overworld ↔ house)
- 2048 Integration: Grid puzzle with merge mechanics affecting mining capabilities



