# Bookmarks Application

A Django application to manage and share bookmarks. This project was built step-by-step to implement core Django features such as user authentication, editable user profiles, and password management.

This project serves as a showcase of backend development skills, including Django model creation, view and form handling, and user authentication workflows.

## 🚀 Features

- **Full User Authentication System**:
    - User registration, login, and logout (using username or email).
    - Password change and password reset via email.
    - Flexible Login: Users can authenticate using either their username or email address via a custom authentication backend.
- **Editable User Profiles**: Users can create and edit their own profiles, including personal information and a profile photo.
- **Django Admin Integration**: Custom admin views for managing application models.
- **Media File Handling**: User-uploaded profile photos are managed via Django's media handling system.
- **User Feedback Messages**: Provides immediate feedback to users on actions like profile updates using Django's messages framework.
- **Social Authentication (Optional)**: Integration capabilities for social login providers (e.g., Google, Facebook) using `social-auth-app-django`.

## 🛠️ Skills & Technologies Demonstrated

By building this project, the following skills and technologies have been applied:

### Backend Development (Python & Django)
- **Django ORM**: Designing relational database models (One-to-One for user profiles).
- **View Logic**: Implementing function-based views for user registration, profile editing, and the main dashboard.
- **Django Auth Framework**: Utilizing Django's built-in authentication views and framework for secure user management, including custom authentication backends.
- **Forms**: Creating and validating Django ModelForms for user registration and profile editing.
- **Dependency Management**: Using `uv` and `pyproject.toml` to manage project dependencies like `Pillow`, `python-decouple`, and `social-auth-app-django`.

### Project Best Practices
- **Version Control with Git**: Adhering to the Conventional Commits specification for a clean, declarative Git history.
- **Standardized Editor Settings**: Using `.editorconfig` to maintain consistent formatting.
- **Dependency Locking**: Ensuring reproducible builds with `uv.lock`.
- **Environment Separation**: Using `.gitignore` to separate source code from user-uploaded media, local database files, and local development certificates.

## 🤖 AI Collaboration

This project was built with the assistance of an AI coding agent (`pi`) acting as a pair-programming partner. Collaborating with the AI allowed for:
- **Accelerated Feature Development**: Rapidly implementing standard Django features like user registration, password reset flows, and social authentication.
- **Code Review & Best Practices**: Applying standard conventions, structuring the project, and maintaining a clean Git commit history.
- **Custom Skill Development**: Creating project-specific `pi` skills to automate the generation of conventional commit messages and README updates, streamlining the development workflow.
- **Public Session Logs**: Sanitized session logs of the AI collaboration are included in the repository, showcasing the iterative development process and providing transparency.

## 💻 Setup & Installation

1. Clone the repository:
   ```bash
   git clone <your-repo-url>
   cd django-social-bookmarks
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