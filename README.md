# django_shop

Приложение онлайн-магазина.

## Quickstart

Run the following commands to bootstrap your environment:

    sudo apt-get install -y git python3-venv python3-pip vim
    git clone https://github.com/rushanqa210488/django_shop.git

    python3 -m venv venv
    source venv/bin/activate
    pip3 install -r requirements/dev.txt

    cp .env.template .env
    while read file; do
        export "$file"
        done < .env

Run the app locally:

    python manage.py runserver --settings=myshop.settings.dev

Run the app with gunicorn:

    gunicorn  myshop.wsgi -b 0.0.0.:8001

