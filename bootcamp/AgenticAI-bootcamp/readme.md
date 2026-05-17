
# 🤖 AI Builder Workshop
## AI Builder Workshop: GenAI & Agentic AI Solutions

> **A hands-on workshop for IT professionals** — brainstorm, design, build, test, and deploy your own AI agent. Walk away with a working solution live on your GitHub profile and a community of AI builders behind you.

---

## 📅 Event Details

| | |
|---|---|
| **Date** | Saturday, July 18, 2025 |
| **Time** | 9:00 AM – 12:00 PM |
| **Location** | Greater Toronto Area *(exact address shared with confirmed registrants)* |
| **Seats** | Limited |

---

## 🎯 Who Should Attend

This workshop is designed for IT professionals who are curious about building real AI solutions. You will get the most out of this session if you:

- Work as a software developer, engineer, or IT professional
- Have familiarity with Software Development Lifecycle (SDLC) concepts
- Are a tech lead, solution architect, or technical team member
- Have basic Python familiarity (writing and running scripts)
- Are eager to build something real — not just watch a demo

No prior AI or machine learning experience is required.

---

## 🗓️ Agenda

| Time | Session |
|------|---------|
| **9:00 – 9:30 AM** | ☕ Morning coffee & pre-workshop networking |
| **9:30 – 9:50 AM** | 🧠 GenAI & Agentic AI — the essentials |
| **9:50 – 10:10 AM** | 💡 Brainstorm & plan your use case |
| **10:10 – 10:25 AM** | 🗺️ Design your agentic workflow |
| **10:25 – 11:10 AM** | 💻 Build & test your AI agent |
| **11:10 – 11:30 AM** | 🚀 Deploy & publish to GitHub |
| **11:30 AM – 12:00 PM** | 🤝 Career guidance & community networking |

### Session Breakdown

**☕ Morning Coffee & Networking (9:00 – 9:30 AM)**
Grab a coffee, meet fellow builders, and settle in. Connect with attendees, mentors, and the BIOM Research Group team before the session kicks off.

**🧠 GenAI & Agentic AI — The Essentials (9:30 – 9:50 AM)**
A quick, practical introduction to what GenAI is, how large language models (LLMs) work, what makes an AI agent, and how agentic workflows think, plan, and act autonomously. No fluff — just what you need to start building.

**💡 Brainstorm & Plan Your Use Case (9:50 – 10:10 AM)**
Define a real problem you want to solve with AI. Identify your agent's inputs, outputs, and responsibilities. Think SDLC — requirements first, code second.

**🗺️ Design Your Agentic Workflow (10:10 – 10:25 AM)**
Map out your agent's decision graph using LangGraph. Define nodes, edges, and tool calls. Understand how Anthropic Claude and OpenAI models fit into your solution architecture.

**💻 Build & Test Your AI Agent (10:25 – 11:10 AM)**
Core hands-on time. Implement your agent with LangGraph, integrate Anthropic Claude or OpenAI, run it, debug it, and iterate. Mentors are available throughout to help you move fast.

**🚀 Deploy & Publish to GitHub (11:10 – 11:30 AM)**
Package your solution, write a README, and push to your GitHub profile. Every attendee leaves with a live, shareable AI project demonstrating real builder skills.

**🤝 Career Guidance & Networking (11:30 AM – 12:00 PM)**
Get feedback on your project, explore open-source AI opportunities with BIOM Research Group, and connect with mentors and fellow builders in the GTA tech community.

---

## 🛠️ What You Will Build

By the end of this 2-hour workshop you will have:

- ✅ Built a working AI agent that performs multi-step reasoning or task execution
- ✅ Integrated at least one LLM (Anthropic Claude or OpenAI GPT)
- ✅ Designed and implemented an agentic workflow using LangGraph
- ✅ Published your complete solution to your personal GitHub repository
- ✅ Demonstrated end-to-end SDLC skills applied to GenAI development

---

## 🧰 Technologies & Tools

- **LangGraph** — agentic workflow orchestration
- **Anthropic Claude API** — reasoning and language capabilities
- **OpenAI API** — alternative / complementary LLM integration
- **Python 3.11+** — primary development language
- **GitHub** — version control and public portfolio publishing
- **VS Code / Cursor** — recommended development environment

---

## 💻 Pre-Workshop Laptop Setup Guide

**Complete all setup steps before arriving on the day.** The workshop moves fast and setup time is not included in the 2-hour session. If you run into issues, reach out to the organizer in advance.

Estimated setup time: **45–60 minutes**

---

### 1. Python Setup

Python 3.11 or higher is required.

#### Install Python

1. Go to [https://www.python.org/downloads/](https://www.python.org/downloads/)
2. Download the latest **Python 3.11+** installer for your operating system (Windows, macOS, or Linux)
3. Run the installer
   - **Windows:** check the box **"Add Python to PATH"** before clicking Install
   - **macOS/Linux:** Python may already be installed; verify with the step below
4. Verify the installation by opening a terminal and running:

```bash
python --version
# or
python3 --version
```

You should see output like `Python 3.11.x` or higher.

#### Create a virtual environment

It is best practice to isolate project dependencies in a virtual environment.

```bash
# Create a project folder
mkdir ai-builder-workshop
cd ai-builder-workshop

# Create a virtual environment
python -m venv venv

# Activate it
# macOS / Linux:
source venv/bin/activate

# Windows (Command Prompt):
venv\Scripts\activate.bat

# Windows (PowerShell):
venv\Scripts\Activate.ps1
```

#### Install required packages

With your virtual environment activated, install the core workshop packages:

```bash
pip install langgraph langchain langchain-anthropic langchain-openai openai anthropic python-dotenv
```

Verify the key packages installed correctly:

```bash
python -c "import langgraph; import anthropic; import openai; print('All packages installed successfully')"
```

---

### 2. GitHub Account & Repository Setup

You will push your finished agent to GitHub at the end of the workshop. Set this up in advance.

#### Create a GitHub account (if you don't have one)

1. Go to [https://github.com](https://github.com)
2. Click **Sign up** and create a free account
3. Verify your email address

#### Install Git

- **Windows:** Download from [https://git-scm.com/download/win](https://git-scm.com/download/win) and run the installer
- **macOS:** Run `git --version` in Terminal — macOS will prompt you to install developer tools if Git is not present
- **Linux (Ubuntu/Debian):** `sudo apt install git`

Verify:

```bash
git --version
```

#### Configure Git with your identity

```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```

#### Create a repository for the workshop

1. Log in to GitHub and click the **+** icon → **New repository**
2. Name it `ai-builder-workshop` (or any name you prefer)
3. Set it to **Public** so your work is visible as a portfolio piece
4. Check **"Add a README file"**
5. Click **Create repository**

#### Authenticate Git with GitHub

The easiest method is a Personal Access Token:

1. Go to GitHub → **Settings** → **Developer settings** → **Personal access tokens** → **Tokens (classic)**
2. Click **Generate new token**
3. Give it a name, set expiry to 90 days, and check the **repo** scope
4. Copy the token and store it somewhere safe (you will not see it again)
5. When prompted for a password during `git push`, paste this token

---

### 3. VS Code Setup

VS Code is the recommended editor for the workshop.

#### Install VS Code

1. Go to [https://code.visualstudio.com](https://code.visualstudio.com)
2. Download and install the version for your OS

#### Install recommended extensions

Open VS Code, press `Ctrl+Shift+X` (Windows/Linux) or `Cmd+Shift+X` (macOS) to open the Extensions panel, then search for and install:

| Extension | Purpose |
|-----------|---------|
| **Python** (by Microsoft) | Python language support, linting, IntelliSense |
| **Pylance** | Fast Python type checking |
| **Jupyter** | Run and explore `.ipynb` notebooks |
| **GitLens** | Enhanced Git history and blame |
| **GitHub Copilot** *(optional)* | AI pair-programmer to help during the workshop |
| **Prettier** | Code formatting |
| **ENV** (by IronGeek) | Syntax highlighting for `.env` files |

#### Open your project folder in VS Code

```bash
# From your terminal, inside your project folder:
code .
```

Select your virtual environment as the Python interpreter:
- Press `Ctrl+Shift+P` → type `Python: Select Interpreter` → choose the `venv` environment you created

---

### 4. Anthropic Claude Account & API Setup

The workshop uses Anthropic Claude as a primary LLM. You need an API key.

#### Create an Anthropic account

1. Go to [https://console.anthropic.com](https://console.anthropic.com)
2. Click **Sign up** and create a free account
3. Verify your email address

#### Get your API key

1. In the Anthropic Console, go to **API Keys** in the left sidebar
2. Click **Create Key**
3. Give it a name like `ai-workshop`
4. Copy the key — it starts with `sk-ant-...`
5. Store it securely (you will not be able to view it again)

> ⚠️ **Never commit your API key to GitHub.** Always load it from an environment variable or `.env` file.

#### Add billing (required to make API calls)

Free accounts require a small credit top-up to use the API:

1. Go to **Settings** → **Billing** in the Anthropic Console
2. Add a payment method and purchase a small credit amount (USD $5 is more than enough for the workshop)

#### Store your API key locally

In your project folder, create a file called `.env`:

```
ANTHROPIC_API_KEY=sk-ant-your-key-here
```

Load it in Python:

```python
from dotenv import load_dotenv
import os

load_dotenv()
api_key = os.getenv("ANTHROPIC_API_KEY")
```

#### Verify your setup

```python
import anthropic

client = anthropic.Anthropic()
message = client.messages.create(
    model="claude-opus-4-5",
    max_tokens=64,
    messages=[{"role": "user", "content": "Say hello in one sentence."}]
)
print(message.content[0].text)
```

#### Optional — Install the Claude desktop app

While not required for coding, having the Claude app available is useful for prompting experimentation:

1. Go to [https://claude.ai/download](https://claude.ai/download)
2. Download and install the app for your OS
3. Sign in with your Anthropic account

---

### 5. OpenAI Account & API Setup

OpenAI models serve as an alternative or complementary LLM during the workshop.

#### Create an OpenAI account

1. Go to [https://platform.openai.com](https://platform.openai.com)
2. Click **Sign up** and create a free account
3. Verify your email address

#### Get your API key

1. In the OpenAI Platform dashboard, go to **API keys** in the left sidebar
2. Click **+ Create new secret key**
3. Give it a name like `ai-workshop`
4. Copy the key — it starts with `sk-...`
5. Store it securely

#### Add billing

1. Go to **Settings** → **Billing**
2. Add a payment method and add a small credit (USD $5 covers the workshop)

#### Add your OpenAI key to your `.env` file

```
ANTHROPIC_API_KEY=sk-ant-your-key-here
OPENAI_API_KEY=sk-your-openai-key-here
```

#### Verify your setup

```python
from openai import OpenAI

client = OpenAI()
response = client.chat.completions.create(
    model="gpt-4o-mini",
    messages=[{"role": "user", "content": "Say hello in one sentence."}]
)
print(response.choices[0].message.content)
```

---

### 6. Final Pre-Workshop Checklist

Run through this checklist the evening before the workshop to make sure everything is ready.

```
[ ] Python 3.11+ installed and accessible from terminal
[ ] Virtual environment created and activated
[ ] langgraph, anthropic, openai, python-dotenv packages installed
[ ] GitHub account created and Git configured
[ ] Workshop repository created on GitHub
[ ] VS Code installed with Python and Pylance extensions
[ ] Anthropic Console account created with billing enabled
[ ] Anthropic API key saved in .env file and tested
[ ] OpenAI Platform account created with billing enabled
[ ] OpenAI API key saved in .env file and tested
[ ] .env file is listed in your .gitignore (so keys are never committed)
[ ] Both API verification scripts run without errors
[ ] Laptop is charged and charger packed
```

#### Add `.env` to `.gitignore`

Create a `.gitignore` file in your project root with the following content:

```
.env
venv/
__pycache__/
*.pyc
.DS_Store
```

---

## 🌱 What Comes Next — BIOM Research Group

After the workshop, standout attendees will be invited to contribute to **open-source AI projects hosted by BIOM Research Group**. This is an opportunity to:

- Work on real, impactful AI research projects alongside other builders
- Grow a meaningful open-source contribution history
- Collaborate with a community of AI practitioners in the GTA and beyond
- Continue developing your GenAI and Agentic AI skills on live projects

More details will be shared during the career guidance session at the end of the workshop.

---

## ❓ Questions?

If you encounter setup issues before the event or have questions about the workshop, please reach out to the organizers in advance. Contact details will be shared in your registration confirmation email.
