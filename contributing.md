

# Contributing to JobPortal

---

## 1. Setup

git clone <repo>
cd jobportal
python -m venv venv

# Windows
venv\Scripts\activate

# Mac/Linux
# source venv/bin/activate

pip install -r requirements.txt

2. Run Project
python manage.py migrate
python manage.py runserver

3. Coding Rules
Follow PEP8 (Python standard)
Use clean and readable code
Use meaningful variable and function names
Keep functions small and modular

4. Commit Convention

Use clear commit messages:

feat: add login system
fix: fix apply job bug
refactor: improve code structure

5. Project Structure
jobportal/
│
├── accounts/
├── jobs/
├── applications/
│
├── templates/
├── static/
│
├── manage.py
6. Pull Request Guidelines
Describe what you changed
Test before pushing
Keep code clean and organized
7. Create Project (if starting new)
django-admin startproject jobportal
cd jobportal

python manage.py startapp accounts
python manage.py startapp jobs
python manage.py startapp applications

8. Notes
Always run migrations after changing models
Keep database schema consistent
Follow project structure strictly