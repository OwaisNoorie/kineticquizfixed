# KineticQuiz — 

This version intentionally follows the visual structure of the supplied KineticQuiz screenshot:
- compact top navigation
- large light-gray hero area
- black statistics card on the right
- four assessment-mode cards
- restrained typography and purple accent
- question-bank section below the fold
- notes section

It is not the previous large "QuizLab" landing-page design.

## Features
- DOCX / JSON upload
- Drag and drop
- Four assessment modes
- Single and multiple correct questions
- Instant answer feedback
- Score and percentage
- Detailed review
- Local question-bank persistence
- Local notes
- Best score
- JSON template download

## DOCX format
Use a structure such as:

Q1. What is Snowpipe?
A. Continuous loading
B. Dashboard
C. Role
D. Package
Answer: A
Explanation: ...

Q2. Which are Snowflake features?
A. Streams
B. Tasks
C. Photoshop
D. Stages
Answer: A, B, D
Explanation: ...

## JSON
{
  "questions": [
    {
      "question": "What is Snowpipe?",
      "type": "single",
      "options": ["A","B","C","D"],
      "answer": ["A"],
      "explanation": "..."
    }
  ]
}

## Run
Open index.html directly or use:
python -m http.server 8000

DOCX extraction uses Mammoth through a CDN.
