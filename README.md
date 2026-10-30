# Agentic AI Lab Practicals

Hands-on labs for building AI agents with the **OpenAI Agents SDK** in Google Colab.
The same three experiments are given for three AI providers. Pick the one that matches the API key you have.

| Provider | Cost | Keys needed |
|---|---|---|
| [OpenAI](openai/) | Paid | `OPENAI_API_KEY`, `TAVILY_API_KEY` (Expt 3) |
| [Google Gemini](gemini/) | Free | `GEMINI_API_KEY`, `TAVILY_API_KEY` (Expt 3) |
| [Groq](groq/) | Free, no card | `GROQ_API_KEY`, `TAVILY_API_KEY` (Expt 3) |

## What you will build

| Expt | Topic | You will learn |
|---|---|---|
| 1 | **Your first AI agent** | Fact Checker and Tweet Bot: agent = name + instructions + model, run with `Runner` |
| 2 | **AI agent with memory** | Market Research Assistant that understands follow-up questions (`SQLiteSession`) |
| 3 | **AI agent with tools** | Live web search (Tavily) plus a calculator / Code Interpreter tool |

## Open a notebook in Colab

Click a link, then use **File → Save a copy in Drive** so you can run and edit your own copy.

| | OpenAI | Gemini | Groq |
|---|---|---|---|
| Expt 1 | [Open](https://colab.research.google.com/github/iftekarpatel/AI-Agent-Notebooks-bkbirla/blob/main/openai/notebooks/Agent_expt1_openai.ipynb) | [Open](https://colab.research.google.com/github/iftekarpatel/AI-Agent-Notebooks-bkbirla/blob/main/gemini/notebooks/Agent_expt1_gemini.ipynb) | [Open](https://colab.research.google.com/github/iftekarpatel/AI-Agent-Notebooks-bkbirla/blob/main/groq/notebooks/Agent_expt1_groq.ipynb) |
| Expt 2 | [Open](https://colab.research.google.com/github/iftekarpatel/AI-Agent-Notebooks-bkbirla/blob/main/openai/notebooks/Agent_expt2_openai.ipynb) | [Open](https://colab.research.google.com/github/iftekarpatel/AI-Agent-Notebooks-bkbirla/blob/main/gemini/notebooks/Agent_expt2_gemini.ipynb) | [Open](https://colab.research.google.com/github/iftekarpatel/AI-Agent-Notebooks-bkbirla/blob/main/groq/notebooks/Agent_expt2_groq.ipynb) |
| Expt 3 | [Open](https://colab.research.google.com/github/iftekarpatel/AI-Agent-Notebooks-bkbirla/blob/main/openai/notebooks/Agent_expt3_openai.ipynb) | [Open](https://colab.research.google.com/github/iftekarpatel/AI-Agent-Notebooks-bkbirla/blob/main/gemini/notebooks/Agent_expt3_gemini.ipynb) | [Open](https://colab.research.google.com/github/iftekarpatel/AI-Agent-Notebooks-bkbirla/blob/main/groq/notebooks/Agent_expt3_groq.ipynb) |

## Lab sheets (copy-paste, step by step)

Prefer typing the code yourself? Open a lab sheet in your browser. Every step has a **Copy** button, the expected result and a check.

- [Lab sheet 1: OpenAI + Gemini](lab-sheets/Agentic_AI_Lab_Practicals.html)
- [Lab sheet 2: Groq edition](lab-sheets/Agentic_AI_Lab_Practicals_Groq.html)

When GitHub Pages is switched on, the landing page is `index.html`.

## Repository layout

```
openai/
  notebooks/        Agent_expt1_openai.ipynb … expt3
  training-notes/   01–03 trainer notes (.docx)
gemini/
  notebooks/        Agent_expt1_gemini.ipynb … expt3
  training-notes/   00 free-key guide, 01–03 trainer notes (.docx)
groq/
  notebooks/        Agent_expt1_groq.ipynb … expt3
lab-sheets/         interactive copy-paste lab sheets (.html)
index.html          landing page for GitHub Pages
```

## Setting up your keys in Colab

1. Click the **key icon** in Colab's left sidebar, then **+ Add new secret**.
2. Use the exact name (for example `GROQ_API_KEY`), paste your key as the value, and switch **Notebook access** on.

| Key | Get it from |
|---|---|
| `OPENAI_API_KEY` | https://platform.openai.com/api-keys |
| `GEMINI_API_KEY` | https://aistudio.google.com/apikey |
| `GROQ_API_KEY` | https://console.groq.com/keys |
| `TAVILY_API_KEY` | https://app.tavily.com |

> **Never** paste an API key into a notebook cell, and never commit a `.env` file to GitHub. Always use Colab Secrets.
