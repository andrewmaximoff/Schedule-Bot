# [Schedule](http://t.me/timetable_kpi_bot) telegram bot on [Heroku](https://www.heroku.com/)
The project was created as a coursework on the discipline 'Software Engineering'. Lecture schedule in a telegram using 
a bot.  
#### Features:
- Schedule of classes for your group by days and weeks.
- Teacher's schedule.
- Exam Schedule.

## Installing
You need the latest version of `pip` to deploy the project on the local machine.
Install virtualenv:
```commandline
$ pip install --upgrade virtualenv
```

Cloning repo:
```commandline
$ git clone https://github.com/qiwiGremL1n/Schedule-Bot
$ cd Timetable-bot
```

Created virtualenv:
```commandline
$ virtualenv -p python3 venv
```
Open `/Timetable-bot/venv/bin/active` and add:
```commandline
TOKEN='Your bot token'
export TOKEN
  
DATABASE_URL='Your database URL'
export DATABASE_URL

FLASK_APP=app.py
export FLASK_APP

FLASK_DEBUG=0
export FLASK_DEBUG

SECRET_KEY='Your secret key'
export SECRET_KEY

```

Activate virtual environment:
```commandline
$ source venv/bin/activate
```

Now install required python packages:
```commandline
(venv) $ pip install -r requirements.txt
```

Start bot polling:
```commandline
(venv) $ flask run
```
