# 🧬SkillDNA — Skill Model Specification

**Version:** 1.0.0  
**Status:** Production Foundation  
**Project:** SkillDNA

---

# 1. Purpose

SkillDNA measures real-world ability through evidence rather than relying primarily on resumes, certificates, self-declared skills, or quizzes.

The system converts:

**Tasks → Evidence → Performance → AI Analysis → Skill Scores → Confidence → Growth → SkillDNA**

---

# 2. Core Principle

A skill score must represent demonstrated capability.

SkillDNA therefore evaluates:

1. Accuracy
2. Speed
3. Complexity
4. Consistency
5. Problem Solving
6. Adaptability
7. Improvement
8. Practical Application

No single test should permanently define a person's skill.

---

# 3. SkillDNA Structure

Each skill contains:

- skill_id
- skill_name
- category
- subskills
- current_score
- confidence
- level
- evidence_count
- evidence_quality
- evidence_diversity
- recent_performance
- historical_performance
- growth_rate
- growth_momentum
- consistency_score
- practical_application_score
- strengths
- weaknesses
- skill_gaps
- related_skills
- last_assessed_at
- algorithm_version

---

# 4. Skill Categories

## 4.1 Programming

Examples:

- HTML
- CSS
- JavaScript
- Python
- Java
- C
- C++
- SQL
- Git
- APIs
- Data Structures
- Algorithms

## 4.2 Data

Examples:

- Data Analysis
- Statistics
- Data Cleaning
- Visualization
- SQL Analytics
- Machine Learning
- Data Interpretation

## 4.3 AI

Examples:

- Prompt Engineering
- Machine Learning
- Model Evaluation
- AI Integration
- Generative AI
- AI Problem Solving

## 4.4 Communication

Examples:

- Writing
- Presentation
- Explanation
- Documentation
- Professional Communication

## 4.5 Problem Solving

Examples:

- Logical Reasoning
- Debugging
- Algorithmic Thinking
- System Thinking
- Decision Making

## 4.6 Professional Skills

Examples:

- Teamwork
- Leadership
- Time Management
- Adaptability
- Project Management
- Collaboration

---

# 5. Evidence Hierarchy

SkillDNA uses an evidence hierarchy.

| Level | Evidence | Initial Reliability |
|---|---|---:|
| E0 | Self Declaration | 0.10 |
| E1 | Basic Quiz | 0.25 |
| E2 | Structured Assessment | 0.45 |
| E3 | Practical Task | 0.65 |
| E4 | Real Project | 0.80 |
| E5 | Verified Real-World Performance | 0.95 |

Higher-level evidence has greater influence.

However, lower-level evidence remains useful for discovering potential skills.

---

# 6. Evidence Object

Each evidence record should contain:

```json
{
  "evidence_id": "EV-001",
  "user_id": "USR-001",
  "skill_id": "javascript",
  "type": "practical_task",
  "level": "E3",
  "score": 82,
  "accuracy": 88,
  "speed": 74,
  "complexity": 80,
  "consistency": 79,
  "problem_solving": 86,
  "adaptability": 72,
  "improvement": 81,
  "practical_application": 84,
  "source": "skill_challenge",
  "created_at": "2026-01-01T00:00:00Z"
}
