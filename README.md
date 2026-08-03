# Introducción a Business Intelligence — Semester 2026-II

**Universidad EAFIT** | Business Intelligence Course
Instructor: Lina María Sepúlveda

## Overview

This repository contains course materials, assignments, and the semester-long project for *Introducción al BI*. Students progressively build an application using SQL, Python, Streamlit, and Oracle Cloud.

## Course Structure

The project is organized into three progressive *retos* (challenges):

1. **Reto 1 — SQL Foundations**: Data modeling and querying over the app schema.
2. **Reto 2 — Python & Streamlit**: Building the application interface, initially hardcoded, then connected to SQL logic.
3. **Reto 3 — Full Integration**: Oracle Cloud connectivity, audit logging, and a complete working application.


## Tech Stack

- **Database**: Oracle Cloud Autonomous Database (ADBG07)
- **Backend**: Python (Anaconda), `oracledb` (thick mode)
- **Frontend**: Streamlit
- **IDE**: PyCharm, SQL Developer
- **Diagramming**: draw.io (diagrams.net)

## Repository Structure

```
├── retos/
│   ├── reto1-sql/
│   ├── reto2-streamlit/
│   └── reto3-integracion/
├── materials/
├── docs/
└── README.md
```

## Evaluation

| Component | Weight |
|---|---|
| Workshops (x3) | 15% |
| Midterms (x2) | 40% |
| Final Project | 30% |
| Attendance | 15% |

## Schedule

Sessions run Mondays and Wednesdays, 3:00–4:30 p.m., July 13 – November 3, 2026. Final project presentations: November 11, 2026.

## Setup

1. Install Anaconda and Oracle Instant Client (`23_26`).
2. Configure the Oracle wallet for mTLS authentication (campus IP whitelisting required).
3. Set up your group's database user (`Gxx_Exx` pattern).
4. Install dependencies: `pip install -r requirements.txt`

## License

Educational use — Universidad EAFIT.
