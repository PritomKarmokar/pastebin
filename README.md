## Initial Setup

1. Clone the project and change into the project directory
   ```shell
   $ git clone git@github.com:PritomKarmokar/pastebin.git
   $ cd pastebin
   ```

2. Create and activate python virtual environment
   ```shell
   $ python3 -m venv venv
   $ source venv/bin/activate
   ```

3. Install project dependencies
   ```shell
    $ pip install --upgrade pip
    $ pip install -r requirements.txt 
   ```

4. Create and update the configuration in `.env` file from `.env.example`
   ```shell
   $ cp .env.example .env
   ```
   Now edit the `.env` file for your local configuration

## Points to be noted while running the project 
- An .env file is required to run the project.
- In the `.env` file, the `DB_HOST` value must be the name of the postgres service name (e.g. `DB_HOST=_postgres`)

# Optional
## If you want to fresh start

1. Create a repository 
```shell
    $ mkdir pastebin
    $ cd pastebin
```

2. Now create virtual environment following the `Initial Setup` no 2 

3. Copy the requirements.txt file (it has necessary packages for working with django postgres along with .env configurations)
- Run
```shell
    $ pip install -r requirements.txt
```

4. Start a fresh new django project 
```shell
    $ django-admin startproject pastebin .
```
5. Configure the `settings.py` file with .env and postgres database configuration following the `pastebin/settings.py`
6. Create the database accordingly and make necessary changes as your need.