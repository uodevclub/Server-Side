# Spring 2016 Week 2 - Server-Side
Learning how to make a server-side application with Flask

### Introduction
Today we will be making a server-side program using [Flask](http://flask.pocoo.org/ "Flask Site"), which is a Python microweb framework that makes it easy to get a server up and running.

### Setting Up

First, you want to create a folder on your local computer where your project will "live". Navigate to this directory and create a python file, app.py, that will be the foundation of your Flask app.
Python has a great tool called [Virtualenv](https://virtualenv.pypa.io/en/latest/ "Virtual Env for Python") that helps you create isolated environments for your Python projects. Go ahead and install virtualenv using Python's package manager, pip.
```
pip install virtualenv
```
After you have installed virtualenv you can create a "container" for your flask project and install flask by running the commands:
```
virtualenv <venv name>
<venv name>/bin/pip install flask
```
where `<venv name>` is whatever you want to name your container (typically "venv"). Next, you want to start your virtual environment with the command:
```
source <venv name>/bin/activate
```
Now you're ready to start coding!  

### Running the Flask App
Execute your app.py by running `python app.py` and you should see something like:
```
* Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)
* Restarting with stat
* Debugger is active!
```

Your server is up and running!

To make calls using the API functions you wrote, start the flask server and run ```curl <url of localhost>/person?q=<handle of user you want to search>```
