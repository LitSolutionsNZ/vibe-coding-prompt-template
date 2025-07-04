# 🚀 Vibe-Coding Workflow: AI-Powered MVP Development

<div align="center">

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)
[![Buy Me A Coffee](https://img.shields.io/badge/☕-Buy%20Me%20A%20Coffee-yellow)](https://www.buymeacoffee.com/alpyalayg)

**Build an MVP in hours, not months – guided end-to-end by AI.**

</div>

---

## Quick Start TLDR
ChatGPT or whatever you code with: 

1) Drag the first doc into your prompt window
Follow the attached promp

2) Do the same for the other docs - Rinse and Repeat

3) Make the App:
a) Web - See Web\Web-Process.md
b) Mobile App - See Mobile\Android-Process.md



## 🎯 What This Does
Turn any app idea into working code through 4 AI-powered stages:

| # | Stage | Goal | Output |
|---|-------|------|--------|
| 1️⃣ | **Research** | Validate market & tech landscape | Research findings |
| 2️⃣ | **Define**  | Clarify product scope | PRD (Product Requirements) |
| 3️⃣ | **Design**  | Decide how to build | Technical Design doc |
| 4️⃣ | **Build**   | Generate & test code | Working MVP |

---

## 🏃 Quick Start

**The Entire Workflow in 30 Seconds**

| Step | What You Do | Time | Result |
|:---:|-------------|:----:|--------|
| 📚 | Copy prompts → Answer questions | 20 min | Research doc |
| 📝 | Define your app idea | 15 min | PRD doc |
| 🏗️ | Choose technical approach | 15 min | Tech Design doc |
| 🤖 | Generate AI instructions | 10 min | NOTES.md |
| 💻 | Tell AI: *"Read NOTES.md and build"* | 1-3 hrs | **Working MVP!** |

**That's it!**

---

## ✅ Prerequisites

**🤖 AI Platform** (choose one)
- [AI Studio](https://studio.google.com) ⭐ - Best free limits (60 req/min)
- [Claude](https://claude.ai) - High quality (30 msg/day free)
- [ChatGPT](https://chat.openai.com) - Versatile (GPT-3.5 free)
- [Gemini](https://gemini.google.com) - Google's LLM (generous free tier)

**💻 AI-Enabled IDE** (choose one)
- [Cursor](https://cursor.sh) ⭐ - Purpose-built for AI coding
- VS Code + [GitHub Copilot](https://github.com/features/copilot) - Popular combo
- [Windsurf](https://codeium.com/windsurf) - Privacy-focused
- [Cline](https://marketplace.visualstudio.com) - Open source VS Code extension

**🛠 Basic Requirements**
- Any modern browser
- 2-4 hours of time
- Zero coding experience needed!

---

## 📋 The 4-Step Workflow

**Transform your idea into a working MVP through these guided steps:**

### 1️⃣ Deep Research 🔍
<details>
<summary><b>Validate your idea with AI-powered market research</b> • 20-30 min • Creates <code>research-*.txt</code></summary>

**What this does:** Analyzes market opportunity, competitors, and technical feasibility

**How it works:**
1. Copy the entire `part1-deepresearch.md` file
2. Paste into any AI platform (AI Studio, Claude, ChatGPT, etc.)
3. Answer 5-6 questions about your idea (tailored to your experience level)
4. AI generates comprehensive research on market, competitors, and implementation options
5. Save the output as `research-[YourAppName].txt`

</details>

### 2️⃣ Product Requirements (PRD) 📝
<details>
<summary><b>Define exactly what you're building</b> • 15-20 min • Creates <code>PRD-*.md</code></summary>

**What this does:** Transforms your idea into clear, actionable product specifications

**How it works:**
1. Copy `part2-prd-generator.md` into a new Gemini chat
2. Attach your research findings when prompted
3. Answer questions about features, users, and success metrics
4. AI creates a professional PRD document
5. Save as `PRD-[YourAppName]-MVP.md`

</details>

### 3️⃣ Technical Design 🏗️
<details>
<summary><b>Plan the technical architecture</b> • 15-20 min • Creates <code>TechDesign-*.md</code></summary>

**What this does:** Decides the tech stack and implementation approach

**How it works:**
1. Copy `part3-tech-design-generator.md` into a new Gemini chat
2. Attach your PRD (required) and research (optional)
3. Answer questions about platform, complexity, and constraints
4. AI designs the technical architecture
5. Save as `TechDesign-[YourAppName]-MVP.md`

</details>

### 4️⃣ Generate AI Agent Instructions 🤖
<details>
<summary><b>Create a blueprint for your AI coding assistant</b> • 5-10 min • Creates <code>NOTES.md</code></summary>

**What this does:** Converts all previous docs into step-by-step coding instructions

**How it works:**
1. Copy `part4-generate-notes-for-agent.md` into a new Gemini chat
2. Attach both PRD and Technical Design documents
3. AI creates detailed implementation instructions
4. Save the output as `NOTES.md`

</details>

</div>

### 5️⃣  Build with AI IDE 💻
<details>
<summary>Time 1-3 hrs • Tool Your AI IDE • Output Working MVP</summary>

#### ➊ Project Setup
1. Create a project folder → add a `docs` subfolder  
2. Move generated files:  
   ```
   docs/research-*.txt
   docs/PRD-*.md
   docs/TechDesign-*.md
   NOTES.md        (in root, not docs)
   ```
3. Open the folder in your AI-enabled IDE

#### ➋ Create AI Agent Rules
File name depends on IDE:

| IDE | Rule File |
|-----|-----------|
| Cursor | `.cursorrules` |
| GitHub Copilot | `copilot-instructions.md` |
| Windsurf | `.windsurfrules` |
| Cline | `.clinerules` |

Paste into the rule file:
```text
You are building an MVP based on documented requirements.
Read NOTES.md first – it is your implementation guide.
Build features incrementally and test each one.
Explain what you're doing in simple terms.

# IMPORTANT:
# Always read [project-name].md before writing any code.
# After adding a major feature or completing a milestone, update [project-name].md.
# Document the entire database schema in [project-name].md.
# For new migrations, make sure to add them to the same file.
```
Replace `[project-name]` with something like `my-app.md`.

#### ➌ Kick-off Prompt (pick one)

| Level | Prompt |
|-------|--------|
| Vibe-Coder | *"I'm a non-technical founder. Read NOTES.md, explain the project, then guide me step-by-step."* |
| Learner | *"Read NOTES.md, explain the tech stack, teach me as we build."* |
| Developer | *"Read NOTES.md + docs/, confirm architecture, start Phase 1."* |

#### ➍ Handy Follow-Up Prompts
```
Let's implement [Feature] – outline plan first.
I'm getting error ____ – debug with me.
Show me how to test [Feature].
Explain this code in plain English.
List remaining tasks from NOTES.md.
```

#### ➎ Finish Line
After all features pass tests:
1. Generate a polished `README.md` (setup & run instructions)  
2. Add `.env.example` with required vars  
3. Walk through full user journey  
4. Deploy (see Tech Design) 🎉
</details>

---

## 📁 Project Structure (after Step 5)
```text
your-app/
├─ docs/
│  ├─ research-YourApp.txt
│  ├─ PRD-YourApp-MVP.md
│  └─ TechDesign-YourApp-MVP.md
├─ NOTES.md
├─ README.md   ← generated by AI
├─ src/…       ← code files (AI-generated)
└─ …
```

---

## 💡 Pro Tips
- Be specific in your answers – detail super-charges AI.  
- Start small; add features later.  
- Test after each major change.  
- Ask *why* – AI will gladly explain.

### Common Pitfalls
| ❌ Pitfall | ✅ Fix |
|-----------|-------|
| Skipping research | Complete **Step 1** – it shapes everything. |
| Feature creep | Stick to the PRD MVP list. |
| Chasing perfect code | Ship, then iterate. |

---

## 🚨 Troubleshooting

### Common Issues & Quick Fixes

| Problem | Solution |
|---------|----------|
| **"Gemini starts deep research in Step 1"** | Turn OFF Deep Research mode → Use regular chat |
| **"AI ignores my documents"** | Explicitly say: *"Read the attached PRD first, then..."* |
| **"Lost track of progress"** | Ask: *"List all completed features and show remaining tasks from NOTES.md"* |
| **"Features don't match PRD"** | Tell AI: *"This doesn't match the PRD. Re-read [feature] requirements."* |

### Emergency Resets

**If AI is completely off-track:**
```
STOP. Let's reset:
1. Re-read NOTES.md completely
2. Tell me what we're building in one sentence
3. List what's been built so far
4. What's the next step according to NOTES.md?
```

---

## 🤝 Contributing
PRs & issues welcome! Improve prompts, share success stories, add edge-cases.

---

## 📜 License
Released under the [MIT License](LICENSE).

---

<div align="center">

**The goal isn't perfect code on the first try – it's a working MVP you can iterate on.**  
Every great app starts somewhere. Yours starts **now**. 🚀

</div>
