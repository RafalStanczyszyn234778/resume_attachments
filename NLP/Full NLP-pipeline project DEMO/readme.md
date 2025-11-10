# Video Emotion Analyzer

> University-supervised project for Content Intelligence Agency

**Status:** Demo available (YouTube) — code artifacts not published.

---

## Table of contents
- [Project overview](#project-overview)
- [Demo](#demo)
- [Features](#features)
- [Architecture & pipeline](#architecture--pipeline)
- [Models](#models)
- [My responsibilities (contributions)](#my-responsibilities-contributions)
- [Tech stack](#tech-stack)
- [Frontend visualizations](#frontend-visualizations)
---

## Project overview
This project is a modular pipeline that analyzes emotion in videos and visualizes results in an interactive frontend. The pipeline is organized as:

```
video -> transcript -> feature extraction -> emotion classification -> frontend visualization
```

The demo shows how a user can paste a video link, choose a timeframe and model, and view emotion intensity across the timeline, an emotion distribution, and colour-coded sentences with timestamps. A feedback mechanism lets users flag wrong labels and submit suggested data for continuous retraining.


## Demo
[**YouTube demo**]`(https://www.youtube.com/watch?v=PAUj3tKDWq4&feature=youtu.be)`

[Click here to watch the demo on YouTube](https://www.youtube.com/watch?v=PAUj3tKDWq4&feature=youtu.be)


---

## Features
- Paste a video link (YouTube) and select a timeframe to analyze.
- Choose from three model tiers: **starter**, **creator**, **enterprise**.
- Timeline visualization showing emotion intensity aligned with video playback.
- Interactive colour-coded pie chart with emotion distribution.
- Sentence-level colour-coded transcript with timestamps.
- Feedback form to report incorrect labels and propose new training data.
- Modular codebase enabling separate model, feature-extraction, and visualization components.

---

## Architecture & pipeline
**High-level stages:**
1. **Video ingestion** — accept a video URL and (optionally) a timeframe.
2. **Transcript generation** — automatic speech recognition / subtitle extraction.
3. **Feature extraction** — tokenization, timestamps, auxiliary features (pause length, speaker changes, etc.).
4. **Emotion classification** — transformer-based model(s) that output emotion labels and intensity scores per sentence/segment.
5. **Frontend visualization** — interactive timeline, pie chart, sentence highlighting and feedback UI.

**Deployment targets:** containerized with Docker; deployed to Azure for hosting APIs and frontend.

---

## Models
- **Starter** — BERT-based emotion classifier (NLP model). Lower compute and fewer emotion classes; optimized for real-time-ish inference and lower cost.
- **Creator** — LLM-augmented model with expanded emotion taxonomy and contextual reasoning.
- **Enterprise** — LLM-based, largest emotion set and more nuanced intensity scoring.

---

## My responsibilities (contributions)
I worked on this project as part of a 5-person team over 16 weeks (8 weeks focused on model development, 8 weeks on deployment). My primary contributions:
- Created one of the tested and suggested **BERT transformer** models used for emotion classification (training, evaluation, and inference code).
- Developed the **frontend & visualization** components (timeline charts, interactive pie chart, colour-coded sentence view).
- Managed the Python package with **Poetry**.
- Wrote and maintained **unit tests** for core components.

Supervision: university-supervised project for the Content Intelligence Agency.

---

## Tech stack
- **Languages & libraries:** Python, HTML (frontend)
- **Package management:** Poetry
- **Containerization:** Docker
- **Cloud / hosting:** Azure
- **Other tools:** unit testing frameworks (pytest)

---


## Frontend visualizations (details)
- **Timeline intensity graph:** Plots per-segment emotion intensity across the video timeline; clicking on a point syncs the video to that timestamp.
- **Emotion distribution pie chart:** Hover or click to inspect counts and percentages; each slice is colour-coded and interactive.
- **Sentence-level view:** Sentences are colour-coded by predicted emotion; clicking a sentence jumps the video to its timestamp and shows the model score.

The visualization code is written in HTML and integrates with the back-end API for live results.

---



