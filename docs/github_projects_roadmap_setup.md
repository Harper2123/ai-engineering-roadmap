# GitHub Projects Setup Guide for AI Engineering Roadmap

This document explains how to set up a free agile-style project management system using:

- GitHub Repositories
- GitHub Issues
- GitHub Projects
- GitHub Milestones
- GitHub Labels
- GitHub Issue Templates
- Notion as a high-level dashboard only

The purpose is to make your AI Engineering learning journey feel like a real engineering project.

---

# 0. Recommended Setup Structure

Use this structure:

```text
GitHub Account
├── Repository 1: ai-engineering-roadmap
│   ├── GitHub Issues
│   ├── GitHub Project
│   ├── Sprint reviews
│   ├── Reading tasks
│   ├── Roadmap docs
│   └── Links to actual project repos
│
└── Repository 2: ml-prediction-service
    ├── Actual Phase 1 code
    ├── README
    ├── notebooks
    ├── src
    ├── tests
    └── Docker/API files
```

Create two repositories now:

1. `ai-engineering-roadmap`
2. `ml-prediction-service`

The first is your agile tracker. The second is your actual Phase 1 project repository.

---

# 1. Create the Roadmap Repository

## Repository Name

```text
ai-engineering-roadmap
```

## Repository Description

```text
Long-term AI Engineering learning and project roadmap using books, projects, GitHub Issues, milestones, and agile sprint tracking.
```

## Visibility

Recommended:

```text
Public
```

Reason: this can become part of your portfolio. It shows discipline, planning, and long-term execution.

Choose `Private` only if you do not want others to see your learning plan yet.

## Initialize Repository

Select:

```text
Add a README file: Yes
Add .gitignore: None
Choose a license: MIT License
```

## Why MIT License?

For the roadmap repo, MIT is fine because it is mostly notes, templates, and process. Later, for code-heavy repositories, MIT is also simple and portfolio-friendly.

## Initial README Content

After creating the repo, open `README.md` and replace it with this:

```markdown
# AI Engineering Roadmap

This repository tracks my long-term AI Engineering learning journey using books, projects, GitHub Issues, milestones, and agile sprint planning.

## Goal

Build deep, practical AI Engineering skills through consistent reading, serious projects, and documented engineering work.

## Strategy

I am not rushing for a job switch. The goal is to develop long-term capability in:

- ML systems
- Deep learning
- Transformers
- LLM applications
- RAG systems
- AI agents
- Evaluation and reliability
- Multimodal AI systems

## Execution Method

This roadmap follows a lightweight agile workflow:

- Phases act as product areas
- Epics represent major learning/project blocks
- Issues represent actionable work
- Sprints are 2 weeks long
- Milestones represent phase completion
- GitHub Projects is used for sprint tracking

## Current Phase

Phase 1: ML Systems + Production ML

## Main Phase 1 Project

ML Prediction Service

Repository: TODO

## Roadmap

| Phase | Focus | Project | Status |
|---|---|---|---|
| Phase 1 | ML Systems + Production ML | ML Prediction Service | Active |
| Phase 2 | Deep Learning + Transformers | Transformer Text Classifier | Not Started |
| Phase 3 | LLM Apps + RAG | Personal Knowledge RAG System | Not Started |
| Phase 4 | Agents + Tool Use | AI Research Assistant | Not Started |
| Phase 5 | Evaluation + Reliability | LLM Evaluation Dashboard | Not Started |
| Phase 6 | Flagship Specialization | Multimodal AI Research Copilot | Not Started |

## Sprint Cadence

- Sprint length: 2 weeks
- Sprint capacity: 12–18 effort points
- Sprint planning: Sunday
- Sprint review: End of sprint
- Sprint retrospective: End of sprint

## Definition of Progress

Progress is counted only when it produces one of the following:

- Notes
- Code
- Experiment result
- Report
- Demo
- Release
```

---

# 2. Create the Phase 1 Project Repository

## Repository Name

```text
ml-prediction-service
```

## Repository Description

```text
Production-style machine learning prediction service with data pipeline, baseline model, FastAPI serving, Docker, testing, logging, and documentation.
```

## Visibility

Recommended:

```text
Public
```

Reason: this is your first portfolio project in the AI Engineering roadmap.

## Initialize Repository

Select:

```text
Add a README file: Yes
Add .gitignore: Python
Choose a license: MIT License
```

## Initial README Content

Replace the README with this:

````markdown
# ML Prediction Service

This repository contains a production-style machine learning prediction service built as Phase 1 of my AI Engineering roadmap.

## Project Goal

Build an end-to-end ML system that goes beyond notebook-based modeling.

The system will include:

- Dataset exploration
- Data preprocessing
- Baseline model training
- Model evaluation
- Model artifact saving
- FastAPI prediction service
- Dockerized deployment
- Logging
- Basic monitoring notes
- Tests
- Documentation

## Why This Project Matters

The goal is to practice ML Engineering fundamentals:

- Reproducibility
- Maintainable project structure
- Training-serving consistency
- API-based model serving
- Evaluation and error analysis
- Deployment readiness
- Documentation quality

## Planned Architecture

```text
Raw Data
   ↓
Data Validation / EDA
   ↓
Preprocessing Pipeline
   ↓
Training Script
   ↓
Evaluation
   ↓
Saved Model Artifact
   ↓
FastAPI Prediction Service
   ↓
Dockerized App
```

## Current Status

Status: Not Started

## Tech Stack

Planned:

- Python
- scikit-learn
- pandas
- numpy
- FastAPI
- Uvicorn
- Docker
- pytest
- GitHub Actions

## Folder Structure

Planned:

```text
ml-prediction-service/
├── data/
├── notebooks/
├── src/
│   ├── data/
│   ├── features/
│   ├── models/
│   ├── api/
│   └── utils/
├── tests/
├── artifacts/
├── reports/
├── Dockerfile
├── docker-compose.yml
├── requirements.txt
└── README.md
```

## Roadmap

- [ ] Select dataset
- [ ] Define ML problem
- [ ] Create EDA notebook
- [ ] Build preprocessing pipeline
- [ ] Train baseline model
- [ ] Evaluate model
- [ ] Save model artifact
- [ ] Create FastAPI app
- [ ] Add Docker support
- [ ] Add tests
- [ ] Write final report
- [ ] Tag v1.0 release

## Linked Roadmap

Main roadmap repository: TODO
````

After saving this, go back to the roadmap repo README and replace `TODO` with the link to this repo.

---

# 3. Create the GitHub Project

Create a user-level GitHub Project because this is your personal roadmap.

## Where to Create

Go to:

```text
Your GitHub profile → Projects → New project
```

## Project Name

```text
AI Engineering Roadmap
```

## Project Description

```text
Agile tracker for my long-term AI Engineering roadmap. Tracks phases, books, projects, experiments, sprint work, reviews, and releases.
```

## Project Type / Template

Choose:

```text
Board
```

If GitHub asks for a template, choose a simple board or blank project. Do not choose something too complex.

---

# 4. Configure Project Columns / Statuses

Create these statuses:

```text
Backlog
Ready
Sprint
In Progress
Review
Done
Parked
```

## Column Meanings

| Column | Use it for |
|---|---|
| Backlog | Future tasks and ideas |
| Ready | Refined tasks ready for a future sprint |
| Sprint | Work committed for the current 2-week sprint |
| In Progress | Work actively being done |
| Review | Done but needs checking, cleanup, documentation, or reflection |
| Done | Completed |
| Parked | Useful but not now |

## Working Rule

Do not keep more than:

```text
2 issues in In Progress
```

This prevents scattered work.

---

# 5. Add Custom Fields to the Project

Add these fields.

## Field 1: Phase

Type:

```text
Single select
```

Options:

```text
Phase 1 - ML Systems
Phase 2 - Deep Learning
Phase 3 - LLM Apps + RAG
Phase 4 - Agents
Phase 5 - Evaluation
Phase 6 - Flagship
```

---

## Field 2: Work Type

Type:

```text
Single select
```

Options:

```text
Book
Project
Experiment
Documentation
Review
Bug
Research
```

---

## Field 3: Priority

Type:

```text
Single select
```

Options:

```text
P0 - Critical
P1 - Important
P2 - Normal
P3 - Optional
```

---

## Field 4: Effort

Type:

```text
Number
```

Use only:

```text
1, 2, 3, 5, 8
```

Meaning:

| Points | Meaning |
|---:|---|
| 1 | 15–30 minutes |
| 2 | 30–60 minutes |
| 3 | 1–2 hours |
| 5 | Half-day |
| 8 | Full weekend or multi-day task |

---

## Field 5: Sprint

Type:

```text
Text
```

Use values like:

```text
Sprint 1
Sprint 2
Sprint 3
```

Later, you can switch to GitHub's iteration field if you want.

---

## Field 6: Outcome

Type:

```text
Single select
```

Options:

```text
Notes
Code
Report
Demo
Release
Decision
```

---

## Field 7: Energy

Type:

```text
Single select
```

Options:

```text
Low
Medium
High
```

Use this practically:

| Energy | Good for |
|---|---|
| Low | Reading, notes, cleanup |
| Medium | Simple coding, documentation |
| High | Debugging, architecture, experiments |

---

## Field 8: Target Date

Type:

```text
Date
```

Use sparingly. Do not over-plan every task.

---

# 6. Create Project Views

Create these views inside the same GitHub Project.

## View 1: Sprint Board

Layout:

```text
Board
```

Group by:

```text
Status
```

Filter:

```text
Sprint:Sprint 1
```

Purpose:

```text
Shows only current sprint work.
```

---

## View 2: Full Backlog

Layout:

```text
Table
```

Fields to show:

```text
Title
Status
Phase
Work Type
Priority
Effort
Sprint
Outcome
Energy
Target Date
```

Purpose:

```text
Master list of all planned work.
```

---

## View 3: Phase Roadmap

Layout:

```text
Roadmap
```

Group by:

```text
Phase
```

Purpose:

```text
High-level timeline of phases and milestones.
```

---

## View 4: Reading Queue

Layout:

```text
Table
```

Filter:

```text
Work Type:Book
```

Purpose:

```text
Tracks book chapters and reading tasks.
```

---

## View 5: Build Tasks

Layout:

```text
Board
```

Filter:

```text
Work Type:Project, Experiment, Bug
```

Purpose:

```text
Tracks coding and implementation work.
```

---

## View 6: Reviews

Layout:

```text
Table
```

Filter:

```text
Work Type:Review
```

Purpose:

```text
Tracks sprint reviews, monthly reviews, and phase reviews.
```

---

# 7. Create Labels in `ai-engineering-roadmap`

Go to:

```text
ai-engineering-roadmap → Issues → Labels
```

Create these labels.

## Phase Labels

```text
phase-1-ml-systems
phase-2-deep-learning
phase-3-rag
phase-4-agents
phase-5-evaluation
phase-6-flagship
```

## Type Labels

```text
type-book
type-project
type-experiment
type-docs
type-review
type-bug
type-research
```

## Priority Labels

```text
priority-p0
priority-p1
priority-p2
priority-p3
```

## Status / Helper Labels

```text
blocked
needs-review
good-first-task
stretch-goal
```

## Suggested Colors

| Label group | Color idea |
|---|---|
| Phase labels | Blue shades |
| Type labels | Green shades |
| Priority labels | Red/orange shades |
| Blocked/review | Yellow/purple |

---

# 8. Create Milestones

Go to:

```text
ai-engineering-roadmap → Issues → Milestones → New milestone
```

Create the following milestones.

## Milestone 1

Title:

```text
M1: Phase 1 - ML Prediction Service v1
```

Description:

```text
Complete Phase 1 of the AI Engineering roadmap by building a production-style ML prediction service with data pipeline, baseline model, FastAPI serving, Docker, testing, logging, and documentation.
```

Due date: leave blank for now.

---

## Milestone 2

Title:

```text
M2: Phase 2 - Transformer Text Classifier v1
```

Description:

```text
Complete Phase 2 by studying deep learning and transformers, then building a transformer-based text classification system with evaluation and deployment-ready structure.
```

---

## Milestone 3

Title:

```text
M3: Phase 3 - Personal Knowledge RAG v1
```

Description:

```text
Complete Phase 3 by building a personal knowledge RAG system with document ingestion, embeddings, vector search, citations, evaluation, and latency/cost tracking.
```

---

## Milestone 4

Title:

```text
M4: Phase 4 - AI Research Assistant v1
```

Description:

```text
Complete Phase 4 by building an AI research assistant that can parse papers, extract methods, datasets, metrics, limitations, and generate literature review tables.
```

---

## Milestone 5

Title:

```text
M5: Phase 5 - LLM Evaluation Dashboard v1
```

Description:

```text
Complete Phase 5 by building an evaluation dashboard for prompts, models, RAG pipelines, latency, cost, hallucination rate, and failure categories.
```

---

## Milestone 6

Title:

```text
M6: Phase 6 - Multimodal Research Copilot v1
```

Description:

```text
Complete Phase 6 by building a flagship multimodal AI research copilot connected to computer vision, image analysis, paper RAG, experiment reporting, and underwater image enhancement research.
```

---

# 9. Create Issue Templates

In `ai-engineering-roadmap`, create this folder:

```text
.github/ISSUE_TEMPLATE/
```

Add the following files.

---

## Template 1: `book-reading.md`

```markdown
---
name: Book Reading
about: Track a book chapter or reading task
title: "[Book] "
labels: type-book
---

## Book

## Chapter / Section

## Phase

## Why I am reading this

## Goal

After completing this, I should understand:

- 
- 
- 

## Reading task

- [ ] Read the chapter/section
- [ ] Highlight important concepts
- [ ] Write notes in my own words
- [ ] Write 3 key takeaways
- [ ] Identify one practical connection to the current project

## Notes

## Key takeaways

1. 
2. 
3. 

## Connection to project

How does this reading affect my project?

## Acceptance criteria

- [ ] I can explain the chapter in my own words
- [ ] Notes are written
- [ ] At least one project improvement or idea is identified
```

---

## Template 2: `project-task.md`

```markdown
---
name: Project Task
about: Track a concrete implementation task
title: "[Project] "
labels: type-project
---

## Task

## Phase

## Project

## Why this matters

## Scope

### Included

- 

### Not included

- 

## Implementation steps

- [ ] 
- [ ] 
- [ ] 

## Acceptance criteria

- [ ] Code is implemented
- [ ] Code runs locally
- [ ] Basic verification is done
- [ ] Documentation updated if needed
- [ ] Changes are committed

## Expected output

- [ ] Code
- [ ] Notes
- [ ] Report
- [ ] Demo
- [ ] Release

## Links

Repository:

Branch:

Pull request:

Notes:
```

---

## Template 3: `experiment.md`

```markdown
---
name: Experiment
about: Track an ML/AI experiment
title: "[Experiment] "
labels: type-experiment
---

## Experiment

## Phase

## Project

## Hypothesis

I expect that:

## Setup

Dataset:

Model / method:

Metric:

Baseline:

## Steps

- [ ] Prepare data
- [ ] Run baseline
- [ ] Run experiment
- [ ] Compare results
- [ ] Write conclusion

## Results

| Metric | Baseline | Experiment |
|---|---:|---:|
|  |  |  |

## Observations

- 
- 
- 

## Conclusion

## Decision

- [ ] Keep
- [ ] Reject
- [ ] Retry later

## Links

Code:

Report:

Notebook:
```

---

## Template 4: `documentation.md`

```markdown
---
name: Documentation
about: Track notes, README updates, diagrams, and reports
title: "[Docs] "
labels: type-docs
---

## Documentation task

## Phase

## Project

## Why this document matters

## Sections to write/update

- [ ] 
- [ ] 
- [ ] 

## Acceptance criteria

- [ ] Content is clear
- [ ] Content is technically accurate
- [ ] Examples or diagrams are added if useful
- [ ] Links are updated
- [ ] Final version is committed or saved

## Output location

File/link:
```

---

## Template 5: `sprint-review.md`

```markdown
---
name: Sprint Review
about: Review a completed sprint
title: "[Review] Sprint "
labels: type-review
---

## Sprint

Sprint number:

Dates:

## Sprint goal

## Planned work

- 
- 
- 

## Completed work

- 
- 
- 

## Not completed

- 
- 
- 

## Points planned

## Points completed

## What I learned

- 
- 
- 

## What blocked me

- 
- 
- 

## What went well

- 
- 
- 

## What did not go well

- 
- 
- 

## What I will change next sprint

- 
- 
- 

## Candidate tasks for next sprint

- 
- 
- 
```

---

## Template 6: `bug.md`

````markdown
---
name: Bug
about: Track a bug or broken behavior
title: "[Bug] "
labels: type-bug
---

## Bug description

## Project

## Expected behavior

## Actual behavior

## Steps to reproduce

1. 
2. 
3. 

## Error message / logs

```text

```

## Possible cause

## Fix checklist

- [ ] Reproduce the bug
- [ ] Identify root cause
- [ ] Implement fix
- [ ] Test fix
- [ ] Document if needed

## Links

Code:

Pull request:
````

---

# 10. Create Phase 1 Epic Issues

In `ai-engineering-roadmap`, go to:

```text
Issues → New issue
```

Create these 8 issues manually.

For each one:

- Add it to the `AI Engineering Roadmap` project.
- Assign the milestone `M1: Phase 1 - ML Prediction Service v1`.
- Set the project field `Phase` to `Phase 1 - ML Systems`.

---

## Epic 1

Title:

```text
[Epic] Phase 1 - Project Setup
```

Description:

```markdown
## Goal

Set up the ML Prediction Service project and define the basic project direction.

## Why this matters

This creates the foundation for Phase 1. Without a clean setup, later work will become scattered.

## Child issues

- [ ] Create GitHub repo for ML Prediction Service
- [ ] Create project folder structure
- [ ] Write initial README
- [ ] Select dataset
- [ ] Define problem statement

## Definition of done

- [ ] Project repository exists
- [ ] Folder structure exists
- [ ] README has project goal and planned architecture
- [ ] Dataset is selected
- [ ] Problem statement is written
```

Labels:

```text
phase-1-ml-systems
type-project
priority-p0
```

Milestone:

```text
M1: Phase 1 - ML Prediction Service v1
```

---

## Epic 2

Title:

```text
[Epic] Phase 1 - Book Reading: ML Systems
```

Description:

```markdown
## Goal

Read and extract useful engineering principles from ML systems books.

## Books

- Designing Machine Learning Systems
- Machine Learning Engineering
- Designing Data-Intensive Applications as reference

## Why this matters

The goal is not just to read books, but to convert reading into engineering decisions for the ML Prediction Service.

## Child issues

- [ ] Read Designing ML Systems: Introduction
- [ ] Read Designing ML Systems: ML project lifecycle
- [ ] Read Machine Learning Engineering: ML lifecycle
- [ ] Write notes on ML lifecycle
- [ ] Connect reading to project decisions

## Definition of done

- [ ] Notes are written
- [ ] Key concepts are summarized
- [ ] At least 3 ideas are applied to the project
```

Labels:

```text
phase-1-ml-systems
type-book
priority-p1
```

Milestone:

```text
M1: Phase 1 - ML Prediction Service v1
```

---

## Epic 3

Title:

```text
[Epic] Phase 1 - Data Pipeline
```

Description:

```markdown
## Goal

Create a reliable data pipeline for loading, exploring, splitting, and preprocessing the dataset.

## Why this matters

A production ML system depends on reproducible and well-documented data handling.

## Child issues

- [ ] Load dataset
- [ ] Perform EDA
- [ ] Identify missing values and outliers
- [ ] Create train/validation/test split
- [ ] Build preprocessing pipeline
- [ ] Document data assumptions

## Definition of done

- [ ] Dataset loads successfully
- [ ] EDA notebook/report exists
- [ ] Split logic is reproducible
- [ ] Preprocessing code is modular
- [ ] Data assumptions are documented
```

Labels:

```text
phase-1-ml-systems
type-project
priority-p0
```

Milestone:

```text
M1: Phase 1 - ML Prediction Service v1
```

---

## Epic 4

Title:

```text
[Epic] Phase 1 - Baseline Model
```

Description:

```markdown
## Goal

Train, evaluate, and document a baseline ML model.

## Why this matters

A baseline gives a reference point before making the system more complex.

## Child issues

- [ ] Train simple baseline model
- [ ] Add evaluation metrics
- [ ] Create model comparison table
- [ ] Perform error analysis
- [ ] Save baseline model artifact
- [ ] Write baseline report

## Definition of done

- [ ] Baseline model trains successfully
- [ ] Metrics are calculated
- [ ] Error analysis is written
- [ ] Model artifact is saved
- [ ] Baseline report is complete
```

Labels:

```text
phase-1-ml-systems
type-project
priority-p0
```

Milestone:

```text
M1: Phase 1 - ML Prediction Service v1
```

---

## Epic 5

Title:

```text
[Epic] Phase 1 - API Serving
```

Description:

```markdown
## Goal

Expose the trained model through a FastAPI prediction service.

## Why this matters

AI Engineering requires serving models through clean interfaces, not just training them in notebooks.

## Child issues

- [ ] Create FastAPI app
- [ ] Add /health endpoint
- [ ] Add /predict endpoint
- [ ] Add request/response schema
- [ ] Add input validation
- [ ] Test API locally

## Definition of done

- [ ] FastAPI app runs locally
- [ ] /health endpoint works
- [ ] /predict endpoint returns predictions
- [ ] Invalid inputs are handled
- [ ] API usage is documented
```

Labels:

```text
phase-1-ml-systems
type-project
priority-p0
```

Milestone:

```text
M1: Phase 1 - ML Prediction Service v1
```

---

## Epic 6

Title:

```text
[Epic] Phase 1 - Docker and Deployment Readiness
```

Description:

```markdown
## Goal

Containerize the ML prediction service and make it easier to run consistently.

## Why this matters

A Dockerized service is easier to reproduce, test, and deploy.

## Child issues

- [ ] Write Dockerfile
- [ ] Build Docker image
- [ ] Run API inside Docker
- [ ] Add docker-compose.yml
- [ ] Document Docker setup

## Definition of done

- [ ] Docker image builds successfully
- [ ] API runs inside container
- [ ] docker-compose works
- [ ] Setup instructions are documented
```

Labels:

```text
phase-1-ml-systems
type-project
priority-p1
```

Milestone:

```text
M1: Phase 1 - ML Prediction Service v1
```

---

## Epic 7

Title:

```text
[Epic] Phase 1 - Logging, Testing, and Monitoring
```

Description:

```markdown
## Goal

Add basic engineering reliability through logs, tests, and monitoring notes.

## Why this matters

A production-style ML system should be observable and testable.

## Child issues

- [ ] Add application logging
- [ ] Add prediction latency logging
- [ ] Add unit tests for preprocessing
- [ ] Add API tests
- [ ] Add basic GitHub Actions workflow
- [ ] Write monitoring notes

## Definition of done

- [ ] Logs are generated
- [ ] Latency is tracked
- [ ] Tests run locally
- [ ] GitHub Actions workflow exists
- [ ] Monitoring limitations are documented
```

Labels:

```text
phase-1-ml-systems
type-project
priority-p1
```

Milestone:

```text
M1: Phase 1 - ML Prediction Service v1
```

---

## Epic 8

Title:

```text
[Epic] Phase 1 - Final Release
```

Description:

```markdown
## Goal

Polish the Phase 1 project into a portfolio-ready release.

## Why this matters

A finished project should be understandable, reproducible, and easy to evaluate.

## Child issues

- [ ] Draw architecture diagram
- [ ] Improve README
- [ ] Add screenshots
- [ ] Write final evaluation report
- [ ] Record short demo
- [ ] Tag release v1.0

## Definition of done

- [ ] README is complete
- [ ] Architecture diagram exists
- [ ] Evaluation report exists
- [ ] Demo asset exists
- [ ] GitHub release v1.0 is created
```

Labels:

```text
phase-1-ml-systems
type-docs
priority-p1
```

Milestone:

```text
M1: Phase 1 - ML Prediction Service v1
```

---

# 11. Create Sprint 1 Issues

Create the following individual issues.

Set all of them to:

```text
Milestone: M1: Phase 1 - ML Prediction Service v1
Project: AI Engineering Roadmap
Sprint field: Sprint 1
Status: Sprint
Phase: Phase 1 - ML Systems
```

---

## Issue 1

Title:

```text
[Project] Create GitHub repo for ML Prediction Service
```

Description:

```markdown
## Task

Create the GitHub repository for the Phase 1 project.

## Why

This repository will contain the actual code for the ML Prediction Service.

## Acceptance criteria

- [ ] Repository is created
- [ ] README exists
- [ ] Python .gitignore is added
- [ ] MIT license is added
- [ ] Repository link is added to the roadmap README
```

Fields:

```text
Work Type: Project
Priority: P0 - Critical
Effort: 1
Outcome: Code
Energy: Low
```

---

## Issue 2

Title:

```text
[Project] Create initial project folder structure
```

Description:

````markdown
## Task

Create the initial folder structure for the ML Prediction Service.

## Folder structure

```text
ml-prediction-service/
├── data/
├── notebooks/
├── src/
│   ├── data/
│   ├── features/
│   ├── models/
│   ├── api/
│   └── utils/
├── tests/
├── artifacts/
├── reports/
├── requirements.txt
└── README.md
```

## Acceptance criteria

- [ ] Folder structure is created
- [ ] Empty `.gitkeep` files are added where needed
- [ ] `requirements.txt` is created
- [ ] Changes are committed
````

Fields:

```text
Work Type: Project
Priority: P0 - Critical
Effort: 2
Outcome: Code
Energy: Low
```

---

## Issue 3

Title:

```text
[Docs] Write initial README for ML Prediction Service
```

Description:

```markdown
## Task

Write the initial README for the ML Prediction Service project.

## README should include

- [ ] Project goal
- [ ] Why this project matters
- [ ] Planned architecture
- [ ] Planned tech stack
- [ ] Folder structure
- [ ] Roadmap checklist
- [ ] Link to roadmap repository

## Acceptance criteria

- [ ] README explains the project clearly
- [ ] README has a planned architecture section
- [ ] README has a roadmap checklist
- [ ] README is committed
```

Fields:

```text
Work Type: Documentation
Priority: P1 - Important
Effort: 2
Outcome: Report
Energy: Low
```

---

## Issue 4

Title:

```text
[Project] Select dataset for ML Prediction Service
```

Description:

```markdown
## Task

Select a dataset suitable for building a production-style ML prediction service.

## Dataset requirements

- [ ] Tabular dataset
- [ ] Suitable for classification or regression
- [ ] Publicly available
- [ ] Not too large
- [ ] Has enough features for preprocessing
- [ ] Has clear target variable

## Candidate datasets

- Customer churn
- Credit risk
- Insurance charges
- House prices
- Loan approval
- Employee attrition

## Acceptance criteria

- [ ] Dataset is selected
- [ ] Dataset source is documented
- [ ] Target variable is identified
- [ ] Problem type is defined
- [ ] Dataset is added to project notes
```

Fields:

```text
Work Type: Project
Priority: P0 - Critical
Effort: 2
Outcome: Decision
Energy: Medium
```

---

## Issue 5

Title:

```text
[Docs] Define ML problem statement
```

Description:

```markdown
## Task

Write a clear problem statement for the ML Prediction Service.

## Problem statement should include

- [ ] Business/user problem
- [ ] ML task type
- [ ] Input features
- [ ] Target variable
- [ ] Success metric
- [ ] Expected user of the API
- [ ] Limitations

## Acceptance criteria

- [ ] Problem statement is written
- [ ] Metric is selected
- [ ] Assumptions are documented
- [ ] Problem statement is added to README or reports folder
```

Fields:

```text
Work Type: Documentation
Priority: P0 - Critical
Effort: 2
Outcome: Report
Energy: Medium
```

---

## Issue 6

Title:

```text
[Book] Read Designing Machine Learning Systems - Introduction
```

Description:

```markdown
## Book

Designing Machine Learning Systems

## Chapter / Section

Introduction

## Goal

Understand what makes machine learning systems different from notebook-based ML models.

## Reading task

- [ ] Read the introduction
- [ ] Write notes in own words
- [ ] Identify 3 ideas relevant to the ML Prediction Service
- [ ] Add notes to roadmap repo

## Acceptance criteria

- [ ] Notes are written
- [ ] 3 key takeaways are listed
- [ ] At least one project decision is influenced by the reading
```

Fields:

```text
Work Type: Book
Priority: P1 - Important
Effort: 2
Outcome: Notes
Energy: Low
```

---

## Issue 7

Title:

```text
[Docs] Write notes on ML lifecycle
```

Description:

```markdown
## Task

Write a short note explaining the ML lifecycle from a production engineering point of view.

## Notes should cover

- [ ] Problem framing
- [ ] Data collection
- [ ] Data validation
- [ ] Model training
- [ ] Evaluation
- [ ] Deployment
- [ ] Monitoring
- [ ] Feedback loop

## Acceptance criteria

- [ ] Notes are written in own words
- [ ] Notes are saved in the roadmap repo
- [ ] Notes mention how the ML Prediction Service will follow this lifecycle
```

Fields:

```text
Work Type: Documentation
Priority: P1 - Important
Effort: 2
Outcome: Notes
Energy: Low
```

---

## Issue 8

Title:

```text
[Review] Sprint 1 review
```

Description:

```markdown
## Sprint

Sprint 1

## Dates

Start:

End:

## Sprint goal

Set up the roadmap system and initialize Phase 1 project.

## Planned work

- [ ] Create GitHub repo for ML Prediction Service
- [ ] Create project folder structure
- [ ] Write initial README
- [ ] Select dataset
- [ ] Define problem statement
- [ ] Read Designing ML Systems introduction
- [ ] Write ML lifecycle notes

## Completed work

- 

## Not completed

- 

## Points planned

14

## Points completed

## What I learned

- 

## What blocked me

- 

## What went well

- 

## What did not go well

- 

## What I will change next sprint

- 

## Candidate tasks for next sprint

- 
```

Fields:

```text
Work Type: Review
Priority: P1 - Important
Effort: 1
Outcome: Report
Energy: Low
```

---

# 12. Create a Starter Folder Structure in `ml-prediction-service`

After creating the repo, clone it locally.

```bash
git clone https://github.com/YOUR_USERNAME/ml-prediction-service.git
cd ml-prediction-service
```

Create folders:

```bash
mkdir -p data/raw data/processed notebooks src/data src/features src/models src/api src/utils tests artifacts reports
touch data/raw/.gitkeep data/processed/.gitkeep notebooks/.gitkeep src/data/.gitkeep src/features/.gitkeep src/models/.gitkeep src/api/.gitkeep src/utils/.gitkeep tests/.gitkeep artifacts/.gitkeep reports/.gitkeep
touch requirements.txt
```

Add starter `requirements.txt`:

```txt
pandas
numpy
scikit-learn
matplotlib
fastapi
uvicorn
pydantic
joblib
pytest
python-dotenv
```

Commit:

```bash
git add .
git commit -m "Initialize project structure"
git push
```

---

# 13. Create a Small Notion Dashboard

Since Notion is only high-level, create one page named:

```text
AI Engineering Roadmap Dashboard
```

Description:

```text
High-level dashboard for tracking phases, current sprint, active book, active project, and monthly reflections. Detailed execution is handled in GitHub Projects.
```

Paste this:

```markdown
# AI Engineering Roadmap Dashboard

## Current Focus

Current Phase: Phase 1 - ML Systems  
Current Sprint: Sprint 1  
Current Project: ML Prediction Service  
Current Book: Designing Machine Learning Systems  

## Links

GitHub Roadmap Repo:  
GitHub Project Board:  
Current Project Repo:  
Current Milestone:  

## Phase Progress

| Phase | Project | Status |
|---|---|---|
| Phase 1 | ML Prediction Service | Active |
| Phase 2 | Transformer Text Classifier | Not Started |
| Phase 3 | Personal Knowledge RAG | Not Started |
| Phase 4 | AI Research Assistant | Not Started |
| Phase 5 | LLM Evaluation Dashboard | Not Started |
| Phase 6 | Multimodal Research Copilot | Not Started |

## Current Sprint

Sprint Goal:

Committed Points:

Completed Points:

Blocked:

## Monthly Reflection

What I built:

What I read:

What I learned:

What I will improve:
```

---

# 14. Exact First-Day Checklist

Complete only this first:

```text
[ ] Create ai-engineering-roadmap repo
[ ] Add roadmap README
[ ] Create ml-prediction-service repo
[ ] Add project README
[ ] Create GitHub Project: AI Engineering Roadmap
[ ] Add statuses: Backlog, Ready, Sprint, In Progress, Review, Done, Parked
[ ] Add custom fields
[ ] Create 6 milestones
[ ] Create labels
[ ] Create 8 Phase 1 epic issues
[ ] Create 8 Sprint 1 issues
[ ] Move Sprint 1 issues to Sprint column
[ ] Create Notion dashboard with GitHub links
```

Once this is done, your system is ready. For the first 2–3 sprints, keep it manual and simple. Do not add automation until the workflow feels natural.
