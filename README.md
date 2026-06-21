Django AI Quiz Generator
A Django-based web application that generates quizzes automatically using the OpenAI API. Users can request a quiz on any topic, and the app uses AI to generate relevant multiple-choice questions on the fly.
Features
Generate quizzes dynamically on any topic using OpenAI's API
Django admin panel for managing quizzes and questions
Clean, server-rendered templates (Django Templates)
SQLite database for local development
Unit tests covering core app functionality
Tech Stack
Backend: Django
AI Integration: OpenAI API
Database: SQLite (default, configurable for production)
Frontend: Django Templates (HTML/CSS)
Project Structure
quiz_project/
├── manage.py
├── quiz_project/
│   ├── settings.py
│   ├── urls.py
│   ├── asgi.py
│   └── wsgi.py
└── quiz_app/
    ├── models.py
    ├── views.py
    ├── admin.py
    ├── tests.py
    ├── migrations/
    └── templates/
        └── base.html
Getting Started
Prerequisites
Python 3.10+
An OpenAI API key
Installation
Clone the repository
git clone https://github.com/khadigaah/django-ai-quiz-generator.git
cd django-ai-quiz-generator
Create a virtual environment and activate it
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
Install dependencies
pip install -r requirements.txt
Set up environment variables Create a .env file in the project root:
OPENAI_API_KEY=your_openai_api_key_here
SECRET_KEY=your_django_secret_key
DEBUG=True
Run migrations
python manage.py migrate
Start the development server
python manage.py runserver
Visit http://127.0.0.1:8000/ in your browser
Running Tests
python manage.py test
Future Improvements
[ ] Support for different question types (true/false, fill-in-the-blank)
[ ] User authentication and quiz history
[ ] Export quizzes to PDF
[ ] Difficulty level selection
This project is open source and available under the MIT License.
