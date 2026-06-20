# Contributing to DevCord

First off, thank you for considering contributing to **devcord** project! 🎉

## Code of Conduct

By participating in this project, you agree to maintain a respectful and inclusive environment for everyone.

## How Can I Contribute?

### Reporting Bugs

1. **Check Existing Issues** - Ensure the bug hasn't already been reported
2. **Include Relevant Details**:
   - Django version
   - Python version
   - Browser/OS if frontend-related
   - Error logs/screenshots

### Suggesting Features

1. **Check Feature Requests** - See if it's already been suggested
2. **Explain the Use Case** - How will this feature improve the chat experience?
3. **Consider Scope** - Is this aligned with the project's goals?

### Pull Requests

1. **Fork the Repository**
2. **Create a Feature Branch**: `git checkout -b feature/amazing-feature`
3. **Follow Coding Standards** (see below)
4. **Add/Update Tests** for your changes
5. **Update Documentation** if needed
6. **Submit PR** with clear description

## Development Setup

### Prerequisites
- Python 3.8+
- Django 3.2+
- SQLite

### Installation

```bash
# Clone your fork
git clone https://github.com/your-username/devcord.git
cd devcord

# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run migrations
python manage.py migrate

# Create superuser (optional)
python manage.py createsuperuser

# Run development server
python manage.py runserver
```

## Coding Standards

### Python/Django Style
- Follow [PEP 8](https://www.python.org/dev/peps/pep-0008/)
- Use Django coding style conventions
- Maximum line length: 88 characters (Black formatter)
- Use type hints where appropriate

### Django-Specific Guidelines

#### Models
- Add docstrings to model classes
- Define `__str__` methods
- Use verbose names for fields
- Add proper related_name for ForeignKeys

#### Views
- Use Class-Based Views when appropriate
- Keep views focused and simple
- Use Django REST Framework for APIs
- Handle WebSocket connections in consumers.py

#### Templates
- Use Django template language features
- Extend base templates
- Keep templates simple and readable

## Getting Help

- Check the [README.md](README.md) for basic info
- Review existing issues and PRs
- Ask questions in issue discussions

## Recognition

Contributors will be:
- Listed in the project's CONTRIBUTORS.md
- Acknowledged in release notes
- Given credit for their work

---

Thank you for contributing to making devcord better! 💬
