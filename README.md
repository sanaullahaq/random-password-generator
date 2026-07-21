# django3-random-password-generator

A Django-based web application that generates random passwords with customizable options — password length, uppercase/lowercase letters, numbers, and special characters.

## Features

- **Adjustable length** — Choose password length from 5 to 14 characters (default: 12)
- **Uppercase letters** — Include A–Z in the password pool
- **Numbers** — Include digits 0–9
- **Special characters** — Include `!@#$%^&*`
- **Custom character** — Add a single user-defined character
- **Custom character position** — Place the custom character at the start or end of the password
- **Bootstrap 4.5 UI** — Clean, responsive interface styled with Bootstrap

## Getting Started

### Prerequisites

- Python 3.8
- pip

### Installation

```bash
git clone <repository-url>
cd django3-random-password-generator
pip install -r requirements.txt
python manage.py runserver
```

Open http://127.0.0.1:8000 in your browser.

> **Note:** `DEBUG` is set to `False` by default. For local development, change it to `True` in `password_generator/settings.py`.

## Usage

1. Select the desired password length from the dropdown (5–14).
2. Check any combination of: **Uppercase**, **Numbers**, **Special Characters**.
3. Optionally type a custom character and choose whether it appears at the start or end.
4. Click **Generate Password**.
5. Copy the generated password from the result page.

## Project Structure

```
├── generator/                  # Main app
│   ├── templates/generator/    # HTML templates (home, password, about)
│   ├── views.py                # Password generation logic
│   └── ...
├── password_generator/         # Django project settings
│   ├── settings.py
│   ├── urls.py                 # URL routing
│   └── ...
├── manage.py
├── requirements.txt
├── Procfile                    # Heroku deployment
└── runtime.txt                 # Python version for Heroku
```

## Deployment

The project is configured for Heroku deployment:

```bash
heroku create your-app-name
git push heroku master
```

## Built With

- [Django 3.1](https://www.djangoproject.com/)
- [Bootstrap 4.5](https://getbootstrap.com/)
- [Gunicorn](https://gunicorn.org/) (production server)
- [WhiteNoise](http://whitenoise.evans.io/) (static files)

## License

Distributed under the MIT License. See `LICENSE` for more information.

## Author

**Sanaulla Haq** — Dhaka, Bangladesh
