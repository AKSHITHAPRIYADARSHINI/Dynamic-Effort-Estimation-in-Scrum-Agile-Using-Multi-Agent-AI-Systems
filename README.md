
# Electric Appliances E‑Commerce Platform

This repository contains four AI-assisted multi-agent workflows using Scrum Agile methodology to plan, design, implement, test, and document an Electric Appliances E-Commerce Platform. All work follows iterative Scrum practices and is executed through structured sprints and cross-functional agent collaboration.



## Phase 2: Scrum (Agile Iterative Development)
Four orchestrated methodologies adapted for Scrum sprints:
- AutoGen (Scrum Sprint-Based)
- AutoGen (Scrum Round-Robin)
- LangChain (Scrum Nested Sequential)
- LangChain (Scrum Round-Robin)

Each notebook produces artifacts representing requirement gathering, design, implementation,
testing, and documentation phases - organized by methodology  (Scrum).

---

## Repository Contents

### Phase 2 - Scrum Notebooks:
```
Experiment1_AutoGen_PreDefinedSearch.ipynb
Experiment2_AutoGen_RoundRobin.ipynb
Experiment3_LangChain_NestedSequential.ipynb
Experiment4_LangChain_RoundRobin.ipynb
```

### Configuration & Documentation:
```
requirements.txt
.env
README.md
Presentation
Panapto Video
```

---

##  Methodologies Compared

### Phase 2: Scrum Agile Methodologies
Each notebook adapts Waterfall patterns to Scrum sprints:

| Approach | Behavior Summary |
|---------|------------------|
| Experiment1: AutoGen Pre Defined Search | Predefined ceremony sequence across multiple sprints |
| Experiment2: AutoGen Round-Robin | Collaborative sprint ceremonies with team rotation |
| Experiment3: LangChain Nested Sequential | Scrum Master coordination with explicit feedback loops |
| Experiment4: LangChain Round-Robin | Iterative team collaboration across sprint cycles |

---

# Phase 2: Scrum Agile Methodology

## Scrum Framework Overview

Phase 2 transforms the Waterfall approach into **Scrum Agile** methodology with:

### Scrum Roles:
- **Product Owner**: Manages Product Backlog, prioritizes user stories, accepts work
- **Scrum Master**: Facilitates ceremonies, removes blockers, tracks velocity
- **Development Team**: Cross-functional members (Developer, QA, UI/UX Designer, DevOps)

### Scrum Artifacts:
- **Product Backlog**: Prioritized list of user stories (US-001, US-002, etc.)
- **Sprint Backlog**: User stories selected for current sprint
- **Increment**: Working product delivered each sprint

### Scrum Ceremonies:
- **Sprint Planning**: Select user stories for sprint (based on velocity)
- **Daily Scrum**: Team synchronization (progress, plans, blockers)
- **Sprint Review**: Demo working increment to Product Owner
- **Sprint Retrospective**: Process improvement discussion

### Sprint Structure:
- **Sprint 0**: Product Backlog creation and story point estimation
- **Sprint 1, 2, 3**: 2-week iterations delivering working increments
- **Story Points**: Effort estimation using Fibonacci (1, 2, 3, 5, 8, 13)
- **Velocity**: Story points completed per sprint (typically 20-30)

## Phase 2 Deliverables

### Product Backlog:
- 20-25 user stories in format: "As a [user], I want [feature], so that [benefit]"
- Story IDs (US-001, US-002, etc.)
- Priority levels (High/Medium/Low)
- Business value scores (1-10)
- Story point estimates

### Sprint Planning:
- Sprint Goals for each iteration
- Sprint Backlogs with selected stories
- Velocity-based capacity planning
- Task breakdowns

### Development Artifacts:
- Working increments delivered each sprint
- Implementation approach per user story
- Code structure and technical decisions
- Cross-functional collaboration

### Testing & Quality:
- Test cases created during sprints (~2-3 per story point)
- Continuous testing throughout sprint
- Acceptance criteria verification
- Quality metrics reporting

### Design & UX:
- UI/UX designs for each sprint's features
- Mobile-responsive wireframes
- Consistent design system
- Usability feedback

### DevOps & Infrastructure:
- CI/CD pipeline setup
- Automated deployment
- Environment management (dev, staging, prod)
- Monitoring and security

### Velocity & Metrics:
- Story points completed per sprint
- Average team velocity across sprints
- Burndown charts
- Sprint completion rates

### Retrospectives:
- What went well
- What to improve
- Action items for next sprint
- Process improvements

---

# How to Run the Project

This repo contains **four runnable notebooks** demonstrating different orchestration styles across two methodologies:


## Phase 2 - Scrum Notebooks:
-Experiment1_AutoGen_PreDefinedSearch.ipynb
-Experiment2_AutoGen_RoundRobin.ipynb
-Experiment3_LangChain_NestedSequential.ipynb
-Experiment4_LangChain_RoundRobin.ipynb

All notebooks share one environment and configuration.

---

## 1️⃣ Prerequisites

- Python **3.11**
- Jupyter Notebook or JupyterLab
- Internet access
- An **OpenAI API key** stored in `.env`

Install dependencies from:

```
requirements.txt
```

---

## 2️⃣ Set Up a Virtual Environment

```bash
# macOS / Linux
python3.11 -m venv .venv
source .venv/bin/activate

# Windows (PowerShell)
py -3.11 -m venv .venv
.venv\Scripts\Activate.ps1
```

Upgrade pip:

```bash
python -m pip install --upgrade pip
```

---

## 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

---

## 4️⃣ Create `.env`

Your project root **must** contain:

```ini
OPENAI_API_KEY=YOUR_KEY_HERE
MODEL_NAME=gpt-4
TEMPERATURE=0.7
MAX_TOKENS=2000
PROJECT_NAME=Electric Appliances E‑Commerce Platform
PHASE=Phase_1_Waterfall
METHODOLOGY=Waterfall
MAX_TURNS=2
MAX_ROUNDS=15
LOG_LEVEL=INFO
SAVE_OUTPUTS=true
OUTPUT_DIR=outputs
```

➡️ Do **NOT** commit `.env`.

---

## 5️⃣ Launch Jupyter

```bash
jupyter notebook
# OR
jupyter lab
```

(Optional) If kernel doesn't appear:

```bash
python -m ipykernel install --user --name elecap --display-name "Python 3.11 (elecap)"
```

---


## 6️⃣ Run Any Notebook

### Phase 2 - Scrum:
- `Experiment1_AutoGen_PreDefinedSearch.ipynb`
- `Experiment2_AutoGen_RoundRobin.ipynb`
- `Experiment3_LangChain_NestedSequential.ipynb`
- `Experiment4_LangChain_RoundRobin.ipynb`

Then click:

```
Run → Run All Cells
```

Outputs (design docs, logs, artifacts, sprint reports) will appear in `outputs/` **if**:

```
SAVE_OUTPUTS=true
```

---

## 7️⃣ (Optional) Run Headlessly

Install Papermill:

```bash
pip install papermill
```

Execute:

```bash
papermill ElectricAppliances_AutoGen_PredefinedSearch.ipynb outputs/predefined_executed.ipynb
```

Repeat for the others.

---

## Troubleshooting

| Problem | Fix |
|---------|-----|
| ModuleNotFoundError | Activate venv + reinstall requirements |
| 401 Unauthorized | Your API key is missing or invalid |
| Output folder missing | Create `/outputs` manually |
| Kernel not listed | Re‑install ipykernel |

---
