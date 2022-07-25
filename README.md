# Flasky

## Env Setup

Pull the repo, go to the project directory and execute following commands
```
source bin/activate
export FLASK_APP=project
```

## DB Setup
Change this according to your DB creds
https://github.com/Mahroz/flasky/blob/223a1c4c6dc2ef9dc9f965f4d4c76cb56d720cd5/project/__init__.py#L12

We'll be initializing DB using flask shell. To run flask shell, run: `flask shell` in bash

In flask shell, execute
```
from project import db, create_app, models
db.create_all(app=create_app())
```

## Running Project
In the same environment execute
`flask run`
You will be able to access app at [localhost:5000](http://localhost:5000)
