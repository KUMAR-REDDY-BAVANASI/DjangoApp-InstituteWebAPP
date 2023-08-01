# Simple Django Login, Registration and Institute Project with Mysql Database

An example of Django project with basic user functionality.

## Installing

### Clone the project

```bash
git clone https://github.com/KUMAR-REDDY-BAVANASI/djangoapp-instituteproject.git
cd djangoapp-instituteproject
```

### Install dependencies & activate virtualenv

```bash
pip install -r requirements.txt
source python3.8/bin/activate
```

### Configure the settings (connection to the database, connection to an SMTP server, and other options)

1. Edit `institutepro/settings.py` if you want to develop the project. Create database in your local pc and give your db details like db_name, db_password, db_user as per your requirement

```bash
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'kumardb',
        'USER':'kumar',
        'PASSWORD':'StrongPassword123@'
    }
}
```

### Apply migrations

```bash
python manage.py makemigrations
python manage.py migrate
```

### Running

#### A development server

Just run this command:

```bash
python manage.py runserver 8000
```