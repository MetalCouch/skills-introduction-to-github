# Introduction to GitHub 🚀

[![GitHub Classroom Workflow](https://img.shields.io/badge/GitHub%20Skills-Interactive-brightgreen)](https://skills.github.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Platform: GitHub](https://img.shields.io/badge/Platform-GitHub-blue.svg)](https://github.com)

Welcome to the **Introduction to GitHub** interactive course! This self-paced, hands-on tutorial is designed to teach you the core workflows of Git and GitHub directly within a live repository. 

Guided by automated GitHub Actions, you will learn how to manage branches, commit changes, open pull requests, and merge code.

---

## 📖 Course Overview

This course is designed for beginners who want to learn the fundamental collaborative workflows used by software developers worldwide. Instead of reading dry documentation, you will learn by **doing**. 

As you perform tasks in this repository (like creating a branch or opening a pull request), an automated background bot (GitHub Actions) will instantly review your work and guide you to the next step.

### What You Will Learn:
* 🌿 **Branching**: How to isolate your work safely without affecting the production code.
* 💾 **Commits**: How to save snapshots of your progress with clear messages.
* 🔀 **Pull Requests**: How to propose changes, request feedback, and collaborate.
* 🤝 **Merging**: How to integrate your approved changes back into the main project.

---

## 🛠️ Tech Stack & Architecture

This course is built entirely using native GitHub features, requiring no external tools or local installations.

* **GitHub Actions**: Powers the automated grading and step-by-step progression engine.
* **Markdown**: Used for all course instructions and documentation.
* **Git**: The underlying version control system.

### How It Works Under the Hood

The course progresses dynamically based on repository events:

```
[ Your Action ] ──(Triggers Event)──> [ GitHub Actions Workflow ] ──> [ Updates Instructions / Steps ]
```

1. **Step Content**: Located in `.github/steps/`. These Markdown files contain the instructions for each stage.
2. **Workflows**: Located in `.github/workflows/`. These YAML files listen for specific Git events (e.g., `create` branch, `push` commit, `pull_request` open/close) and trigger the transition to the next step.

---

## 🚀 Getting Started

You can start this course in under 2 minutes. No local setup or command-line experience is required!

### Prerequisites
* A free [GitHub Account](https://github.com/join).

### Installation & Initialization

To start the course, you need to create your own copy of this repository:

1. Scroll to the top of this page and click the **Use this template** button (or click [this link](https://github.com/new?template_name=skills-introduction-to-github&template_owner=MetalCouch) to create a new repository from this template).
2. Select yourself as the **Owner**.
3. Name your repository (e.g., `my-first-github-course`).
4. Set the visibility to **Public** (required for GitHub Actions to run on free accounts).
5. Click **Create repository from template**.
6. Wait about 30 seconds, then **refresh the page**. Your automated guide will post the first set of instructions directly on your new repository's home page or in a Pull Request!

---

## 🎓 Course Roadmap & Steps

The course consists of 5 sequential steps:

| Step | Title | Action Trigger | Key Concept |
| :--- | :--- | :--- | :--- |
| **0** | **Welcome** 👋 | Repository Creation | Introduction to the workspace |
| **1** | **Create a Branch** 🌿 | Branch Creation | Isolating your development environment |
| **2** | **Commit a File** 💾 | File Push | Saving changes with version control |
| **3** | **Open a Pull Request** 🔀 | PR Creation | Initiating code review and collaboration |
| **4** | **Merge Your Pull Request** 🤝 | PR Merge | Integrating features into the `main` branch |
| **X** | **Finish** 🎉 | Merge Complete | Next steps and graduation |

---

## 🛠️ Development & Customization

If you are an educator, team lead, or developer looking to customize this course for your team, you can easily modify the steps and workflows.

### Directory Structure
```
├── .github/
│   ├── steps/                # Markdown files containing step-by-step instructions
│   └── workflows/            # GitHub Actions YAML files orchestrating course logic
├── images/                   # Visual assets used in the markdown steps
└── README.md                 # Course landing page
```

### Modifying Step Instructions
To change the text or instructions for any step, navigate to `.github/steps/` and edit the corresponding `.md` file:
* `0-welcome.md`
* `1-create-a-branch.md`
* `2-commit-a-file.md`
* `3-open-a-pull-request.md`
* `4-merge-your-pull-request.md`
* `X-finish.md`

### Modifying Workflow Logic
The progression logic is controlled by the YAML files in `.github/workflows/`. For example, to change how the "Create a Branch" step is validated, edit `.github/workflows/1-create-a-branch.yml`.

---

## ❓ Troubleshooting

### 1. The course isn't updating or responding to my actions.
* **Check Actions Tab**: Click on the **Actions** tab at the top of your repository. If you see a warning that Actions are disabled, click **Enable Actions**.
* **Public Visibility**: Ensure your repository is set to **Public**. GitHub Actions may not run automatically on private repositories depending on your account settings and limits.
* **Wait a Moment**: GitHub Actions can sometimes take 10–30 seconds to trigger and complete a step. Refresh your page.

### 2. I made a mistake and got stuck.
* You can always delete your created repository and start fresh by clicking **Use this template** again. Don't worry—learning is all about trial and error!

---

## 🤝 Contributing

We welcome contributions to improve this course! If you find a typo, broken link, or have an idea for a new feature:

1. Fork this repository.
2. Create a new branch (`git checkout -b feature/improvement`).
3. Commit your changes (`git commit -m 'Improve step 3 instructions'`).
4. Push to the branch (`git push origin feature/improvement`).
5. Open a Pull Request.

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 💖 Acknowledgments

* Inspired by the official [GitHub Skills](https://skills.github.com/) program.
* Built to help developers take their very first steps into the open-source world.