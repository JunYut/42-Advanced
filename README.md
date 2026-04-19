# 🖥️ 42 Advance

This repository is the central command center for my **42 Advance programme** journey. It contains no source code; instead, it houses the logic, requirements, and tracking for every project module.

## 🗂️ The Standard Hierarchy
To manage multiple complex projects, we use a decoupled 3-tier system:

1.  **The Project (Global Level):** Managed via the [GitHub Project Board]. This groups all subjects.
2.  **The Feature (Parent Issue):** A high-level requirement (e.g., "HTTP/1.1 Parsing") located in **this** repo.
3.  **The Task (Sub-issue):** Granular, code-level tickets nested within the Feature.

---

## 📋 Planning Workflow

### 1. Define the Feature
Before coding, create a formal **Issue** in this repository. 
* Use the **Project Field** to assign it to a specific 42 Subject (e.g., `Project-1`).
* Use **Sub-issues** to break the feature into "Atomic Tasks" (e.g., `ft_split_input`, `handle_signal_void`).

### 2. The "Branch-First" Development
Once a feature is ready to be worked on:
1.  Open the **Feature Issue** in this repo.
2.  Navigate to the **Development** section in the right sidebar.
3.  Click **"Create a branch"**.
4.  **⚠️ Critical:** Change the **Repository destination** from this roadmap repo to your actual **Code Repository** (e.g., `your-username/minishell`).
5.  GitHub will generate a branch name linked to this specific ticket.

---

## 💻 Execution Workflow (Cross-Repo)

### 1. Local Development
Sync the newly created branch to your local machine from within your **Code Repository**:
```bash
git fetch origin
git switch <branch-name-from-roadmap>
```

### 2. Pull Requests & Automation
When the feature is complete, open a Pull Request (PR) in the **Code Repository**. 
* **Auto-Link:** Because the branch was created from the Roadmap Issue, the PR is automatically linked.
* **Closing:** In the PR description, use the keyword to link across repos:
  `Closes your-username/42-Advanced-Roadmap#ID_NUMBER`
* **Result:** Merging the PR in your code repo will automatically close the Feature ticket here and update your Project Board progress.

---

## 📊 Project Board Strategy
The [GitHub Project Board] provides three essential views for the 42 curriculum:

| View | Purpose |
| :--- | :--- |
| **Current Sprint** | Kanban board filtered by `Status: In Progress` across all subjects. |
| **Subject Roadmap** | A timeline view to manage overlapping 42 deadlines and peer-evaluations. |
| **Backlog** | Grouped by `Subject` to see remaining Mandatory vs. Bonus tasks. |
