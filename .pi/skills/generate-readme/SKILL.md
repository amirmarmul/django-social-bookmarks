---
name: generate-readme
description: Generates or updates a README.md file based on the project's codebase, features, and technologies. Use when the user asks to "create a readme", "update the readme", or document the project.
---

# Skill: Generate README

## Instructions

When asked to generate or update a README, follow these steps:

1.  **Analyze Project Context:**
    *   Examine dependency files (e.g., `pyproject.toml`, `requirements.txt`, `package.json`, `uv.lock`) to identify the core technologies and frameworks used.
    *   Review the project structure and main application files (e.g., `urls.py`, `views.py`, `settings.py` in Django) to understand the implemented features and architecture.
    *   Check for existing documentation or comments that describe the project's purpose.

2.  **Determine Structure:**
    *   Ask the user if they have a specific reference or template they would like to use.
    *   If no reference is provided, use a standard professional structure:
        *   **Title & Description:** Project name and a high-level summary.
        *   **🚀 Features:** Bulleted list of key functionalities.
        *   **🛠️ Technologies:** Tech stack and core libraries used.
        *   **💻 Setup & Installation:** Step-by-step guide to run the project locally.

3.  **Draft Content:**
    *   Write the content clearly, focusing on what the project does and how it was built.
    *   Ensure the installation instructions accurately reflect the project's specific setup (e.g., using `uv sync`, `python manage.py`).

4.  **Confirm and Write:**
    *   Present the drafted Markdown content to the user for review.
    *   Ask for feedback or adjustments.
    *   Once approved, use the `write` tool to save the content to `README.md`.
