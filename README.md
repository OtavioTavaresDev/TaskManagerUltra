# 📋 TaskManager Ultra V3

**AI-Powered Task Management System with Full Customization**

![Version](https://img.shields.io/badge/version-3.0-blue) ![License](https://img.shields.io/badge/license-MIT-green) ![Platform](https://img.shields.io/badge/platform-web-lightgrey) ![Language](https://img.shields.io/badge/language-JavaScript-yellow) ![Made with](https://img.shields.io/badge/made%20with-%E2%9D%A4%EF%B8%8F-red)

---

## 🧠 Overview

**TaskManager Ultra V3** is a full-featured Kanban-style task management web application built entirely with **vanilla HTML, CSS, and JavaScript** — no frameworks, no server, no database required. It combines agile workflows with artificial intelligence, allowing users to organize projects, collaborate with teams, and automate processes through a conversational AI assistant powered by OpenAI, Groq, or Google Gemini.

This project was born out of a real professional need: during my internship at **ADEVA AISTHETIKÉ**, I faced challenges with internal organization, follow‑up tracking, and team collaboration. I developed this tool to help myself and my colleagues stay on top of daily tasks, manage client interactions, and ensure no critical activity was overlooked. It quickly became an essential part of our workflow, and I've since refined it into a robust, production‑ready solution.

The application is **offline‑first**, storing all data locally in the browser's `localStorage`, and provides a rich, customizable experience including:

- ✅ Drag‑and‑drop Kanban boards
- ✅ Advanced tasks with checklists, priorities, categories, tags, and assignees
- ✅ Analytical dashboard with productivity charts
- ✅ Interactive calendar
- ✅ Quick notes
- ✅ Dynamic widget dashboard (Central Adeva)
- ✅ Executive mode for high‑priority focus
- ✅ Brain Dump – automatic task creation from free text
- ✅ AI conversational assistant (ChatGPT, Groq, Gemini)
- ✅ Export/Import in **7 formats** (JSON, CSV, XML, YAML, TOML, TXT, HTML)
- ✅ Responsive design (mobile‑first) with light/dark themes
- ✅ Full customization of sidebar navigation and dashboard widgets

---

## 🎯 Purpose & Target Audience

This system is ideal for:

- **Freelancers and consultants** (lawyers, doctors, coaches) managing multiple clients and projects.
- **Small teams** seeking a lightweight, zero‑cost solution with no hosting overhead.
- **Developers** looking for a practical example of a single‑page application (SPA) with local storage, DOM manipulation, and AI API integration.
- **Students** wanting to learn front‑end development, including responsive design, drag‑and‑drop, and chart rendering.

---

## 🚀 Key Features

### 📊 Kanban Boards
- Create, edit, and delete boards with custom colors.
- Dynamic columns (rename, reorder, delete).
- Drag‑and‑drop tasks between columns and internal reordering.
- Board metrics (total tasks, completed, overdue, in progress).

### 📝 Advanced Task Management
- Title, description, due date, priority (Low, Medium, High, Critical).
- Categories and Tags (with custom colors).
- Checklist with checkable items and progress bar.
- Assignee, estimated time, and time spent (hours).
- Favorite tasks.
- Task progress indicator based on checklist completion.

### 📈 Dashboard
- Consolidated statistics: total, completed, overdue, in progress, completion percentage.
- Productivity chart (last 7 days) using **Canvas API**.

### 📅 Calendar
- Monthly view with task indicators.
- Color‑coded dots by priority.

### 📝 Quick Notes
- Create and edit notes with title and content.
- Basic Markdown support (bold, italic, lists, links).

### 🏥 Central Adeva (Customizable Widgets)
- Dynamic widgets displaying metrics like:
  - Pending follow‑ups
  - Clients to contact
  - Campaign ideas
  - Weekly tasks
  - Monthly goals
- **All widgets are user‑configurable** (title, content, and placeholders like `{{totalTasks}}`, `{{todayTasks}}`, `{{followUps}}`, `{{boardsCount}}`).

### 🎯 Executive Mode
- Focused view on:
  - Critical tasks (priority)
  - Overdue tasks
  - Today's tasks
  - Overall completion percentage
- Quick summary for decision‑making.

### 🧠 Brain Dump
- Paste a block of text (ideas, tasks, reminders).
- Automatically splits items by commas, periods, or line breaks.
- Creates tasks in the first available board (or creates a new "Brain Dump" board).

### 🤖 AI Assistant
- Supports **three providers**:
  - **OpenAI** (GPT‑4o, GPT‑4‑turbo, GPT‑3.5‑turbo)
  - **Groq** (Llama 3.3, Llama 3.1, Gemma)
  - **Google Gemini** (Gemini 1.5 Pro, Flash, etc.)
- Persistent chat history.
- Customizable system context (initial instructions).
- File upload to enrich context (.txt, .md, .json).
- Font and color customization for the chat interface.
- Fully responsive.

### ⚙️ Settings (Full Customization)
- **Change application name** (displayed in the sidebar).
- **Manage sidebar tabs**:
  - Add, edit, reorder, and delete tabs.
  - Each tab has an icon, label, and destination page.
- **Manage Central Adeva widgets**:
  - Add, edit, reorder, and delete widgets.
  - Smart placeholders for dynamic data.

### 📤 Export & Import
- **Export** in 7 formats:
  - `JSON` (complete data)
  - `CSV` (task table)
  - `XML` (hierarchical structure)
  - `YAML` (human‑readable)
  - `TOML` (configuration format)
  - `TXT` (plain text summary)
  - `HTML` (visual page)
- **Import** files in JSON, XML, YAML, TOML, or TXT (with JSON content).

---

## 🛠️ Technologies Used

- **HTML5** – Semantic and accessible structure.
- **CSS3** – Responsive styling with CSS variables (light/dark themes), grid, and flexbox.
- **JavaScript (ES6+)** – Business logic, DOM manipulation, event handling, native drag‑and‑drop, Canvas charts.
- **localStorage** – Local data persistence (no server required).
- **External APIs**:
  - OpenAI API
  - Groq API
  - Gemini API
- **Optional CDN Libraries**:
  - [js-yaml](https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js) – for YAML export/import.
  - [@iarna/toml](https://cdn.jsdelivr.net/npm/@iarna/toml@2.2.5/dist/toml.min.js) – for TOML export/import.

---

## 📦 Installation & Setup

### Prerequisites
- Modern web browser (Chrome, Firefox, Edge, Safari).
- Internet connection (to load CDN libraries and make AI API calls – optional).

### Steps
1. **Download** the `TaskManagerAI_ULTRA.html` file or clone this repository.
2. **Open the file** directly in your browser (double‑click or drag into a browser window).
3. **Start using it** – all data is automatically saved to your browser's `localStorage`.

> 💡 *Tip: For the full AI experience, configure your API key in the "AI Assistant" section.*

---

## 🔧 AI Assistant Configuration (Step‑by‑Step)

1. Navigate to the **"AI Assistant"** page from the sidebar.
2. Select the **Provider** (OpenAI, Groq, or Gemini).
3. Choose a **Model** (type or select from the suggestion list).
4. Enter your **API Key** (obtained from the provider's platform).
5. (Optional) Add a **Context** (initial instructions for the AI).
6. (Optional) Upload a context file (.txt, .md, .json).
7. Click **"💾 Save Configuration"**.
8. Now you can start chatting with the assistant.

---

## 🎨 Advanced Customization

### Change Application Name
- Go to **Settings** → **Application Name**.
- Enter the new name and click **Save**.

### Manage Sidebar Tabs
- In **Settings** → **Sidebar Tabs**.
- **Add**: click the "+ Add Tab" button.
- **Edit**: directly modify the label, icon, or target page.
- **Move**: use the ↑ and ↓ arrows to reorder.
- **Delete**: click the ✕ (the "Settings" tab is fixed and cannot be deleted).

### Manage Central Adeva Widgets
- In **Settings** → **Central Adeva Widgets**.
- **Add**: click "+ Add Widget".
- **Edit**: change the title or content.
- **Move**: use the ↑ and ↓ arrows.
- **Delete**: click the ✕.
- **Available placeholders**: `{{totalTasks}}`, `{{todayTasks}}`, `{{followUps}}`, `{{boardsCount}}`.

---

## 📁 Data Structure (localStorage)

All data is stored under the key `adeva_data` with the following structure:

```json
{
  "boards": [
    {
      "id": "abc123",
      "name": "My Project",
      "color": "#0052cc",
      "createdAt": "2026-06-22T10:00:00.000Z",
      "favorite": false,
      "columns": [
        {
          "id": "col1",
          "name": "To Do",
          "order": 0,
          "tasks": [...]
        }
      ]
    }
  ],
  "categories": [...],
  "tags": [...],
  "notes": [...],
  "settings": { "theme": "light" },
  "ia": { ... },
  "appName": "📋 Adeva",
  "sidebarItems": [...],
  "widgets": [...]
}
```

---

## 🔒 Privacy & Security

- **All data stays in your browser** (localStorage).
- No information is sent to external servers except for AI API calls, which are made directly from your browser to the chosen provider.
- Your API key is stored locally and never shared.

---

## 🚦 Roadmap (Planned Features)

- [ ] Cloud sync (Google Drive, Dropbox).
- [ ] Board sharing among multiple users.
- [ ] Push notifications.
- [ ] Full offline mode (Service Worker).
- [ ] Multi‑language support (i18n).

---

## 🤝 Contributing

Contributions are warmly welcome! If you'd like to improve the project:

1. **Fork** the repository.
2. Create a **branch** for your feature (`git checkout -b feature/amazing-feature`).
3. **Commit** your changes (`git commit -m 'Add amazing feature'`).
4. **Push** to the branch (`git push origin feature/amazing-feature`).
5. Open a **Pull Request**.

---

## 📄 License

This project is licensed under the **MIT License** – see the [LICENSE](LICENSE) file for details.

---

## 👨‍💻 Developer

**Otavio Tavares Dev**

- 📧 **Email**: [otaviotavaresdev@gmail.com](mailto:otaviotavaresdev@gmail.com)
- 🐙 **GitHub**: [OtavioTavaresDev](https://github.com/OtavioTavaresDev)
- 💼 **LinkedIn**: (coming soon)

---

## 🙏 Acknowledgments

- The open‑source community for the amazing libraries.
- AI providers (OpenAI, Groq, Google) for democratizing access to artificial intelligence.
- All users who tested and provided valuable feedback.

---

## 💡 Why This Project Exists

During my internship at **ADEVA AISTHETIKÉ**, I realized that our team lacked a unified tool to track daily tasks, follow‑ups, and internal communication. I built this system to address those pain points, and it quickly became the backbone of our daily operations. I decided to open‑source it so that other professionals and teams can benefit from the same efficiency and clarity.

---

**TaskManager Ultra V3 – Organize, automate, and achieve your goals! 🚀**
