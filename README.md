# EVENTEX
Eventex is an Event Manager Web App 

[![Code Health](https://landscape.io/github/andrealmar/eventex/master/landscape.svg?style=flat)](https://landscape.io/github/andrealmar/eventex/master)

[![Build Status](https://travis-ci.org/andrealmar/eventex.svg?branch=master)](https://travis-ci.org/andrealmar/eventex)

## How to get your hands dirty on the code

1. Clone this repo
2. Create a virtualenv with Python 3.5 (virtualenv .venv)
3. Activate virtualenv (source .venv/bin/activate)
4. Install the dependencies (pip install -r requirements.txt)
5. Configure your instance with .env 
6. Execute the tests (python manage.py test)


```
git clone https://github.com/andrealmar/eventex.git wttd
cd wttd
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
cp contrib/env-sample .env
python manage.py test
```

## How to make a deploy

1. Create a Heroku instance (heroku create instancename)
2. Send the configs to Heroku (heroku config:push)
3. Define a SECRET_KEY for your instance (heroku config:set SECRET_KEY=python contrib/secret_gen.py')
4. Define DEBUG=False (heroku config:set DEBUG=False)
5. Configure e-mail service
6. Send your code to heroku (git push heroku master --force)


