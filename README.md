# BRIEF2BUILD
Riphah Uni AI Hackathon - Task 1 | BRIEF2BUILD: Client Brief to Jira Tickets Converter | NEVER ASSUME rule, Source Reference, Jira CSV Export
# BRIEF2BUILD

## AI-Powered Pre-Development Intelligence Engine

BRIEF2BUILD converts natural-language client briefs into structured software requirements, developer tasks and project risk assessments.

Its purpose is to identify ambiguity, missing information and contradictions before software development begins.

## Features

### 1. Requirement Extraction
- Extracts project goals and requirements.
- Identifies vague requirements.
- Detects conflicting statements.
- Identifies missing information.
- Flags undefined integrations and terms.
- Preserves source evidence.

### 2. Developer Task Generation
- Groups requirements into features.
- Generates developer tasks.
- Provides acceptance criteria.
- Records source references.
- Lists dependencies and open questions.
- Leaves unspecified priority, estimate and deadline as "Not specified".

### 3. Project Readiness Intelligence
- Classifies detected risks.
- Identifies scalability, performance, security, availability and reliability concerns.
- Maps risks to tasks using available source evidence.
- Produces READY, READY WITH RISKS or NOT READY assessments.

### 4. Export
- Complete JSON project report.
- Jira-style CSV developer task export.

## Technology Stack

- Python
- Streamlit
- Google Gemini API
- Google Gen AI SDK
- Pandas
- python-dotenv

## Project Structure

```text
BRIEF2BUILD/
├── core/
│   ├── __init__.py
│   ├── requirement_extractor.py
│   ├── task_breakdown.py
│   └── readiness_engine.py
├── app.py
├── requirements.txt
├── README.md
├── .env
└── .gitignore
```

## Installation

1. Install Python 3.10 or later.
2. Open the project folder in a terminal.
3. Create a virtual environment:

```bash
python -m venv venv
```

4. Activate it on Windows:

```powershell
venv\Scripts\Activate.ps1
```

5. Install dependencies:

```bash
pip install -r requirements.txt
```

6. Create a `.env` file in the project root:

```text
GEMINI_API_KEY=YOUR_API_KEY
```

Never publish or share your API key.

## Run the Application

```bash
streamlit run app.py
```

Open the local URL displayed in the terminal.

## Testing

Run the available test scripts:

```bash
python test_extraction.py
python test_edge_cases.py
python test_task_breakdown.py
python test_readiness.py
```

## Important Limitations

- AI-generated task descriptions and acceptance criteria require human review.
- Exact source references do not guarantee that every generated detail is supported by the source.
- Readiness results are rule-based assessments, not guarantees of project success.
- Task impact mapping uses source-text matching and may miss indirect relationships.
- BRIEF2BUILD generates CSV exports; it does not directly create issues in a Jira account.

## Product Principle

No requirement without evidence.
No task without traceability.
No development without clarity.

## Project

BRIEF2BUILD | HAITx Engineering
Development Build 3.0
