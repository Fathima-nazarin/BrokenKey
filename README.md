# ⚡ KeyRush - Typing Speed Test

A no-build typing speed test made with HTML, CSS and vanilla JavaScript. Benchmark your typing speed, watch real-time performance analytics, and help improve the experience. This repository is intentionally shipped with defects for a workshop, hackathon, or contribution event.

## Run it

1. Fork this repository (or create a new repository and upload these files).
2. Open `index.html` in a browser, or run it with VS Code Live Server.
3. Press **Start test** and type the passage.
4. Find an issue, reproduce it, and submit a fix with a short explanation and test steps.

There is no build step and no dependency installation. GitHub Pages can host it as a static site.

## Suggested contribution levels
 
| Level | Focus Areas | What you'll practise |
|---|---|---|
| 🟢 Easy | UI contrast, basic event handling, counter displays, documentation | CSS variables, input events, DOM basics |
| 🟡 Medium | Calculation algorithms, timer lifecycles, paste handling, state persistence | State machines, timing, input edge cases, canvas |
| 🔴 Hard | Concurrency, race condition mitigation, replay modes, visual data mapping | Event timing, async flows, replay engines, data viz |

## Features already present

- 15 / 30 / 60 second rounds
- Passage randomisation and per-character highlighting
- Live WPM, accuracy, error count, and personal best display
- Light/dark theme control
- Live WPM speed progression graph
- Per-key error keyboard heatmap
- Ghost mode entry point (currently a placeholder page)
- Responsive layout and keyboard-friendly controls

Some of these features are intentionally imperfect. That's the challenge: the UI may look finished while the implementation needs investigation.

## 🎯 The Bug Hunt Challenge

This application is intentionally shipped with multiple subtle defects and performance quirks across timer lifecycle handling, user input edge cases, score metrics, and visual rendering. 

Instead of a pre-defined checklist, contributors are challenged to **hunt, reproduce, and report** defects like a real QA engineer and open-source contributor:

1. **Test the Application:** Play rounds of 15s, 30s, and 60s. Try rapid typing, pasting text, backspacing, switching themes mid-game, restarting abruptly, and testing at the zero-second mark.
2. **Investigate the Code:** Dig into `script.js` and `style.css` to locate where logic breaks down or state desynchronizes.
3. **Report the Defect:** If you discover an unlisted bug, open a **Bug Report** using our issue template with reproduction steps.
4. **Get Mentor Approval:** Mentors will verify your findings, assign the difficulty tier (`level:medium` or `level:hard`), and give you the green light to claim and fix it!

*Note: Starter beginner-friendly issues (`level:easy`) are listed on the [Issues Tab](https://github.com/tkmfoss/BrokenKey/issues) to help you get your first PR merged.*

## ⚖️ Independent-Work & AI Policy

**AI assistance is prohibited for every part of this KeyRush challenge.** This includes using AI to inspect the repository, identify or diagnose defects, suggest fixes, generate or edit code, create tests, review a proposed solution, or implement any feature—even partially.

Do not upload, paste, or otherwise provide KeyRush source code, screenshots, bug descriptions, or challenge materials to AI tools. Disable AI coding agents, AI autocomplete, and AI code-review features while working on this challenge.

You may use ordinary editors, browser developer tools, debuggers, and official language/API documentation. Submissions must represent your own independent work. Review [`CONTRIBUTING.md`](CONTRIBUTING.md) for full submission evidence requirements and live verification policies.

## 🚀 FOSSSoC Season 1 Contribution Guidelines

This repository is an official project for **FOSSSoC Season 1 (November Phase)** hosted by **[TKM FOSS](https://github.com/tkmfoss)**.

- 🌐 **Live Demo:** [https://tkmfoss.github.io/BrokenKey/](https://tkmfoss.github.io/BrokenKey/)
- 📋 **Active Issues:** Browse open challenges on the [Issues Tab](https://github.com/tkmfoss/BrokenKey/issues) (tagged `soc-s1`).

---

### 1. How to Claim an Issue
1. Browse open issues tagged with `soc-s1`.
2. Comment `/claim` on an unassigned issue.
3. Our automated bot will immediately assign you if you meet the eligibility criteria.
4. ⚠️ **1-Issue Rule:** You can only have **ONE active claimed issue at any time** across all FOSSSoC repositories. You must have your pull request merged or closed before claiming another.
5. ⏳ **Tiered Inactivity Window:** You have **3 days (72 hours)** for Easy issues, and **5 days (120 hours)** for Medium and Hard issues to open a pull request. If no PR is opened within this window, the bot automatically unassigns the issue to keep opportunities open for others.

---

### 2. How to Raise a New Issue & Work on It
Found an unlisted bug, edge case, or have an idea for an awesome new feature (e.g., sound effects, custom passages, accessibility improvements, word-count mode)? You are strongly encouraged to propose it!

#### Step A: Check Existing Issues & PRs
Before creating a new issue, search the [Issues Tab](https://github.com/tkmfoss/BrokenKey/issues) and [Pull Requests Tab](https://github.com/tkmfoss/BrokenKey/pulls) to make sure someone else hasn't already reported, claimed, or fixed it. Duplicate issues will be closed.

#### Step B: Open an Issue with a Template
1. Go to [New Issue](https://github.com/tkmfoss/BrokenKey/issues/new/choose).
2. Choose either **Bug Report** or **Feature Proposal**.
3. Use a clear, conventional title:
   - For bugs: `fix(scope): concise description of the defect` (e.g., `fix(audio): keystroke audio clips during rapid typing`)
   - For features: `feat(scope): concise description of the proposal` (e.g., `feat(ui): add audio click toggle for keystrokes`)
4. Fill out all template sections: steps to reproduce, expected vs observed behavior, relevant files, and your proposed approach.

#### Step C: Mentor Review & Difficulty Assignment
- A project mentor will review your proposal to verify that it is constructive, non-trivial, and fits the challenge.
- If approved, the mentor will tag your issue with:
  - `soc-s1` label (mandatory for automated leaderboard tracking).
  - The appropriate difficulty tier: `level:easy` (10 pts), `level:medium` (25 pts), or `level:hard` (50 pts).
- ⚠️ **IMPORTANT:** **Do not start coding or submit a PR until a mentor has reviewed and labeled the issue!** PRs linked to unapproved or unlabeled issues cannot be scored by the automated leaderboard.

#### Step D: Claim and Begin Working
- As soon as the mentor adds the labels, comment `/claim` on the issue to assign yourself.
- The standard **1-Issue Rule** applies (you cannot claim if you already have an active assigned issue).
- Your **tiered inactivity clock (3 days for Easy, 5 days for Medium/Hard)** begins once assigned.

---

### 3. How to Submit Your Solution
1. Fork this repository to your personal GitHub account.
2. Clone your fork locally and create a descriptive branch:
   ```bash
   git checkout -b fix/accuracy-counter
   ```
3. Test your changes locally by opening `index.html` in your browser.
4. Commit your changes with clear commit messages and push to your fork.
5. Open a Pull Request targeting `main` of `tkmfoss/BrokenKey`.
6. 🔗 **CRITICAL:** Include `Fixes #<issue_number>` in your pull request description (e.g., `Fixes #2`). This automatically links the issue, closes it upon merge, and ensures the automated leaderboard tracks your score!

---

### 4. Scoring & Points

| Difficulty | Tag | Points | Description |
|---|---|---|---|
| 🟢 Easy | `level:easy` | **10 pts** | Great for getting started |
| 🟡 Medium | `level:medium` | **25 pts** | State, lifecycle, and event edge cases |
| 🔴 Hard | `level:hard` | **50 pts** | Concurrency, replay modes, visual data mapping |

- ⚡ **Early Bird Bonus:** **+5 bonus points** for PRs opened during Week 1 (November 1 – November 7).
- 🌟 **Quality Bonus:** **+5 bonus points** for clean, well-documented code with thorough PR descriptions (awarded via `quality:excellent` label).
- 🛑 **Repository Cap:** Maximum of **5 scored PRs** per repository.

---

## License and attribution

MIT License. This workshop challenge is based on the original project at [ankeshbit/typing-speed](https://github.com/ankeshbit/typing-speed).

