# Flask Template

Flask is a micro framework for creating web application.


## Virtual Environment

Virtual environment `venv` is a tool to manage dependencies for your project and isolate your Python environment.

In `Python 3.3`, you can use Python’s built-in `venv` module to create a virtual environment.

The `virtualenv package` can be installed in Python 3, so it’s up to you which you want to use.

### Creating Virtual Environment

Python 3 come with virtual environment package name `venv`.

1 - Create a project folder : `mkdir project_name`

2 - Move to the project folder : `cd project_name`

3 - Install `venv`

- on Windows : `python3 -m venv env`

- on MacOs :  `python3 -m venv env`

The  `-m venv` option runs the `venv` package from the standard library as a standalone script, passing the desired name as an argument.

### Working with a Virtual Environment

When you want to start using a virtual environment, you have to “activate” it

1 - Activate `env` :

- on Windows : `env\Scripts\activate`

- on MacOs : `source env/bin/activate`

2 - De-Activate `env` :

- on Windows : `env\Scripts\deactivate`

- on MacOs : `source env/bin/deactivate`

### Installing Python Packages with pip

To install Flask into the virtual environment, make sure the `venv` virtual environment is activated, and then run the following command:

   ` pip install flask`

  When you execute this command, pip will install Flask and all of its dependencies.

  You can check what packages are installed in the virtual environment at any time using the pip freeze command:

  `pip freeze`

### Development Web Server

Flask applications include a development web server that can be started with the
flask run command. This command looks for the name of the Python script that
contains the application instance in the FLASK_APP environment variable.

- on Windows :

  `set FLASK_APP=project_name.py`

  `set FLASK_ENV=development`

  `flask run`

- on MacOs :

  `export FLASK_APP=project_name.py`
  
  `export FLASK_ENV=development`

  `flask run`
