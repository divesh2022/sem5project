
# 🛠️ DIT – Developer Integrated Tool

DIT is a Git-inspired version and view control system designed for academic environments. It empowers students to manage their codebases, collaborate on projects, and learn Git workflows while enforcing ethical and educational constraints.

DIT introduces:
- 🎭 Role-based access
- 📝 Editor integration
- 🤖 AI-powered plagiarism detection
- 🧠 Ethical coding enforcement

---

## 📚 Table of Contents

- [🚀 Features](#-features)
- [👥 User Roles](#-user-roles)
- [🧰 Getting Started](#-getting-started)
- [💻 CLI Commands](#-cli-commands)
- [📝 Editor Integration](#-editor-integration)
- [🚫 Restrictions & Ethics](#-restrictions--ethics)
- [🤖 Plagiarism Detection](#-plagiarism-detection)
- [📆 Development Roadmap](#-development-roadmap)
- [🤝 Contributing](#-contributing)
- [📄 License](#-license)
- [🙌 Acknowledgements](#-acknowledgements)

---

## 🚀 Features

✨ DIT offers a structured, ethical, and collaborative coding experience:

- 🧭 Git-like CLI commands (`init`, `add`, `commit`, `push`, `pull`, etc.)
- 🔐 Role-based access control (Student, Team Member, Team Leader, Faculty)
- 🖊️ Integrated code editor with file origin tracking
- ✂️ Paste restriction enforcement (>100 characters blocked)
- 🤖 AI-powered plagiarism detection and feedback
- 🧪 Sandbox mode for ethical scripting exploration
- 🏅 Badge system for achievements and creativity
- 🧑‍🏫 Mentor dashboard for review and guidance

---

## 👥 User Roles

| Role           | Abbr | Capabilities                                                                 |
|----------------|------|------------------------------------------------------------------------------|
| 👨‍🎓 Student        | st   | Create/edit personal repos, limited commit rights                            |
| 👥 Team Member    | tm   | Collaborate on team repos, suggest changes                                   |
| 🧑‍💼 Team Leader    | tl   | Merge, assign tasks, manage branches                                         |
| 🧑‍🏫 Faculty/Mentor | fm   | Read-only access, trigger plagiarism scans, review flagged submissions       |

---

## 🧰 Getting Started

### 🔧 Prerequisites

- 🐍 Python 3.9+
- ⚡ FastAPI
- 🎨 Streamlit (or React for frontend)
- 🗃️ SQLite or PostgreSQL
- 🧬 Git (for repo management)

### 📦 Installation

```bash
git clone https://github.com/your-org/dit.git
cd dit
pip install -r requirements.txt
```

### 🚀 Run the Backend

```bash
uvicorn main:app --reload
```

### 🖥️ Launch the Editor (Streamlit)

```bash
streamlit run editor_interface.py
```

---

## 💻 CLI Commands

```bash
dit init                   # Initialize a new DIT repo
dit add <file>            # Stage a file
dit commit -m "message"   # Commit changes
dit push                  # Push to remote repo
dit pull                  # Pull latest changes
dit status                # Show current repo status
dit log                   # View commit history
```

📁 All metadata is stored in a `.dit/` directory, similar to `.git/`.

---

## 📝 Editor Integration

- 🧷 Files must be created within the DIT editor to be eligible for commit.
- 🚫 External files are blocked via origin metadata checks.
- 🌐 Supports syntax highlighting and multi-language extensions.

---

## 🚫 Restrictions & Ethics

DIT enforces ethical coding practices:

- ❌ Pasting more than 100 characters is blocked.
- ❌ Opening files created outside the editor is restricted.
- ✅ All actions are logged for audit and review.
- 🧪 Sandbox mode available for ethical scripting experiments.

---

## 🤖 Plagiarism Detection

DIT integrates AI-based plagiarism detection:

- 🔍 MOSS or custom AST comparison engine
- 🧠 Detects:
  - Copy-paste patterns
  - Structural similarity
  - Suspicious reuse across users
- 📊 Faculty can view scan results and commit timelines

---

## 📆 Development Roadmap

| Phase     | Duration     | Focus                    |
|-----------|--------------|--------------------------|
| Phase 1   | Days 1–10     | Planning & Architecture  |
| Phase 2   | Days 11–40    | Core System Development  |
| Phase 3   | Days 41–60    | Testing & Refinement     |
| Phase 4   | Days 61–80    | Deployment & Feedback    |
| Phase 5   | Days 81–100   | Documentation & Showcase |

---

## 🤝 Contributing

We welcome contributions from educators, developers, and students! 💡

### 🛠️ How to Contribute

1. 🍴 Fork the repo
2. 🧪 Create your feature branch  
   `git checkout -b feature/YourFeature`
3. 💾 Commit your changes  
   `git commit -m 'Add some feature'`
4. 🚀 Push to the branch  
   `git push origin feature/YourFeature`
5. 📬 Open a Pull Request

📜 Please read our [Code of Conduct](CODE_OF_CONDUCT.md) before contributing.

---

## 📄 License

This project is licensed under the MIT License.  
See the [LICENSE](LICENSE) file for details.

---

## 🙌 Acknowledgements

- 🧠 Inspired by Git and GitHub workflows
- 🎓 Educational support from mentors and faculty
- 🤖 AI integration powered by open-source tools


