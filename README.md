# Bookmarks Application

A Django application to manage and share bookmarks. This project was built step-by-step to implement core Django features such as user authentication, editable user profiles, and password management.

This project serves as a showcase of backend development skills, including Django model creation, view and form handling, and user authentication workflows.

## 🚀 Features

- **Full User Authentication System**:
    - User registration, login, and logout.
    - Password change and password reset via email.
- **Editable User Profiles**: Users can create and edit their own profiles, including personal information and a profile photo.
- **Django Admin Integration**: Custom admin views for managing application models.
- **Media File Handling**: User-uploaded profile photos are managed via Django's media handling system.

## 🛠️ Skills & Technologies Demonstrated

By building this project, the following skills and technologies have been applied:

### Backend Development (Python & Django)
- **Django ORM**: Designing relational database models (One-to-One for user profiles).
- **View Logic**: Implementing function-based views for user registration, profile editing, and the main dashboard.
- **Django Auth Framework**: Utilizing Django's built-in authentication views and framework for secure user management.
- **Forms**: Creating and validating Django ModelForms for user registration and profile editing.
- **Dependency Management**: Using `uv` and `pyproject.toml` to manage project dependencies like `Pillow` and `python-decouple`.

### Project Best Practices
- **Version Control with Git**: Adhering to the Conventional Commits specification for a clean, declarative Git history.
- **Standardized Editor Settings**: Using `.editorconfig` to maintain consistent formatting.
- **Dependency Locking**: Ensuring reproducible builds with `uv.lock`.
- **Environment Separation**: Using `.gitignore` to separate source code from user-uploaded media and local database files.

## 🤖 AI Collaboration

This project was built with the assistance of an AI coding agent (`pi`) acting as a pair-programming partner. Collaborating with the AI allowed for:
- **Accelerated Feature Development**: Rapidly implementing standard Django features like user registration and password reset flows.
- **Code Review & Best Practices**: Applying standard conventions, structuring the project, and maintaining a clean Git commit history.
- **Custom Skill Development**: Creating a project-specific `pi` skill to automate the generation of conventional commit messages, streamlining the development workflow.

## 💻 Setup & Installation

1. Clone the repository:
   ```bash
   git clone <your-repo-url>
   cd bookmarks
   ```

2. Set up a virtual environment and install dependencies:
   ```bash
   uv sync
   ```

3. Run migrations and create a superuser:
   ```bash
   python manage.py migrate
   python manage.py createsuperuser
   ```

4. Run the development server:
   ```bash
   python manage.py runserver
   ```
   Visit `http://127.0.0.1:8000/account/` to view the app.
