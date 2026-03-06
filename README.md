---
title: MCQ Answer Sheet Generator
emoji: 📋
colorFrom: orange
colorTo: yellow
sdk: gradio
sdk_version: "6.5.1"
python_version: "3.10"
app_file: app.py
pinned: false
---

# MCQ Answer Sheet Generator

An app that reads a PDF containing MCQ (multiple choice) questions with options and answers, and generates a clean answer sheet document.

## Features

- Upload any MCQ PDF with questions, options (a/b/c/d), and answers
- Extracts each question and resolves the answer letter to its full answer text
- Generates a downloadable **PDF** or **DOCX** answer sheet
- Handles multi-column PDF layouts automatically

## Output Format

```
Q1. 49th Parallel is the boundary line between which two countries?
Answer - USA and Canada

Q2. The longest day of the year in the Northern Hemisphere occur on _______
Answer - 21st June
```

## Supported PDF Format

Questions must follow this structure:

```
Question: 1. Question text here?
(a) Option 1
(b) Option 2
(c) Option 3
(d) Option 4
Answer: a
```

## Running Locally

```bash
cd question-answer-summarizer
uv sync
uv run app.py
```
