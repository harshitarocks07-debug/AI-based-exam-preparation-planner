# PrepPilot AI

Adaptive AI exam-prep planner (TCS Technology Day & AI Hackathon MVP).

## Run (Windows)

```javascript
cd preppilot-ai
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
ollama list          # confirm a model exists, e.g. llama3.2
streamlit run app.py
```

## How it works

- **Deterministic engines** (SQLite + Python): risk, priority, readiness, planner, what-if.
- **Ollama (local LLM)**: only for explanations, chat, and report insights.
- **Offline-safe**: if Ollama is down, everything still works with local fallbacks.

## Demo story (2-3 min)

1. Dashboard -> readiness, top risk (DSA Graph Traversal).
2. AI Assistant: "What should I study today?"
3. Study Planner -> generate plan.
4. Mark a DSA session **Missed** -> watch risk recalc + replan.
5. Ask the AI about the missed session.
6. What-If Simulator -> raise hours/day, show projection.
7. Reports -> Generate AI Study Report.
