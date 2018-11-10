# dead-simple-flask-app
minimal Flask template

###Build

Setup virtualenv:

	$ pip install virtualenv
	$ virtualenv venv
	$ . venv/bin/activate

Install app dependencies:

	$ pip install -r requirements.txt

###Run

Run app with Gunicorn workers:

	$ gunicorn -w 4 --bind 0.0.0.0:9000 app:app
	[2018-11-10 18:23:01 -0500] [7915] [INFO] Starting gunicorn 19.9.0
	[2018-11-10 18:23:01 -0500] [7915] [INFO] Listening at: http://0.0.0.0:9000 (7915)

Hit app locally: [http://localhost:9000/](http://localhost:9000/)