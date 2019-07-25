Python: mypot
A barebones Django app, which can easily be deployed to Heroku.


Running Locally
Make sure you have Python 3.7 installed locally. To push to Heroku, you'll need to install the Heroku CLI, as well as Postgres.

$ git clone https://github.com/Mwapsam/mypot.git
$ cd mypot

$ python3 -m venv mypot
$ pip install -r requirements.txt

$ createdb python_mypot

$ python manage.py migrate
$ python manage.py collectstatic

$ heroku local
Your app should now be running on localhost:5000.

Deploying to Heroku
$ heroku create
$ git push heroku master

$ heroku run python manage.py migrate
$ heroku open
