# Django <> Next.js - Backend API

The Django Ninja API backend for the Django x Next.js course.


## Getting Started

Clone, create virtual environment, activate it, install requirements, then run:

```bash
git clone https://github.com/codingforentrepreneurs/django-nextjs-backend-api
```

Create virtual environment
```bash
# if mac/linux/wsl
sudo apt install python3.10-venv   # install required package if use linux
python3 -m venv venv

# if windows powershell
c:\Python312\python.exe -m venv
```

Activate virtual environment
```bash
# if mac/linux/wsl
source venv/bin/activate

# if windows powershell
.\venv\Scripts\activate
```

Install requirements
```bash
# If activated, the command line should start with:
# (venv)
pip install pip --upgrade
pip install -r requirements.txt
```

Copy default env
```bash
cp .env.sample .env
```

Generate secret key and put inside .env file
```bash
python -c 'from django.core.management.utils import get_random_secret_key; print(get_random_secret_key())'
```

Run project

```bash
# Using the Rav CLI: https://github.com/jmitchel3/rav
rav run server


# or directly with django
cd src
python manage.py runserver 8001
```


