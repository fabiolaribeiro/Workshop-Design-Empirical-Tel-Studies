# Strawberries & Exam Performance - A Longitudinal Study Workshop

![](./strawberry_student.png)

Does eating a certain amount of strawberries every day improve exam performance over time?

---

## Workshop Goal

The goal of this workshop is not only to test whether strawberries help students, but also to learn how longitudinal data can be analyzed using modern statistical techniques.

---

## Study Design

![](strawberry_study.png)

### Overview

This workshop uses an artificial longitudinal dataset simulating student behavior over an 8‑week university study.

Participants were randomly assigned to different daily strawberry intake groups and repeatedly measured over time.

The dataset was designed for teaching:

- longitudinal data analysis
- repeated measures
- mixed-effects models
- growth trajectories
- multilevel modeling
- visualization of longitudinal trends

---

### Participants

- Total participants: 25 university students
- Study duration: 8 weeks
- Repeated measurements: weekly

Each participant has their own:

- study habits
- stress patterns
- sleep behavior
- compliance level
- learning trajectory

---

### Experimental Groups

| Group | Daily Strawberry Intake |
|---|---|
| Control | 0 g/day |
| Low Dose | 50 g/day |
| Medium Dose | 100 g/day |
| High Dose | 200 g/day |

---

### Measurements Collected Weekly

| Variable | Description |
|---|---|
| participant_id | Unique participant identifier |
| week | Measurement occasion (1–8) |
| group | Experimental condition |
| assigned_strawberries_g | Intended intake per day |
| actual_strawberries_g | Real intake per day |
| study_hours | Weekly study hours |
| sleep_hours | Average sleep per night |
| stress_level | Weekly stress level |
| exam_score | Weekly mock exam score |

---

### Longitudinal Structure

The dataset is in **long format**.

Each row represents:

- one participant
- at one week
- with one measurement occasion

Example:

| participant_id | week | group | exam_score |
|---|---|---|---|
| P01 | 1 | 100g | 71 |
| P01 | 2 | 100g | 73 |
| P01 | 3 | 100g | 74 |

---

### Important Features of the Dataset

The simulation intentionally includes:

- individual differences
- gradual learning effects
- varying stress levels
- imperfect treatment compliance
- realistic noise
- heterogeneous trajectories

---

## Suggested Analyses

Participants may explore:

### Descriptive Analysis
- group means
- distributions
- trajectories

### Visualization
- line plots
- participant trajectories
- group trends over time

### Longitudinal Modeling

Example mixed-effects model:

\[
ExamScore_{it} = \beta_0 + \beta_1 Week_t + \beta_2 Strawberries_{it} + \beta_3 StudyHours_{it} + \beta_4 Stress_{it} + u_i + \epsilon_{it}
\]

# Ethical Considerations

- informed consent
- voluntary participation
- wellbeing-sensitive design
- data anonymization
- ethical handling of longitudinal student data

---

# Workshop Reflection

Imagine your research team has received €1 million in research funding from EATEL to investigate the effects of breathing exercises in Higher Education. **How would you design the study to generate meaningful evidence about whether daily strawberry consumption can improve exam performance over time?**
