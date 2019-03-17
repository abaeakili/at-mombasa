
### Africa's Talking Pre-Workshop Training


## PYTHON FLASK APP WITH AFRICA’S TALKING  API’S – SWAHILIBOX MEETUP

# Done on Saturday, 2nd March, 2019

Have you been looking at how you can start programming but don’t know where to start? maybe this is your year..
Last weekend we held a very successful meetup and I want to let you also benefit by sharing my side experience.

After one week of planning and putting everything in place, we conducted a refresher/introductory course of Python, GIT, Flask and Heroku for preparation of Africa’s Talking Meet-up, where we incorporated their API’s to our Very Simple Flask Application.

The steps below would help you, or anyone from a beginner to an advanced to be able to create a simple application and accomplish same results.

Learners were able to do the following:

## PART 1:
1. Introduction to Python Programming Language
2. Build a Flask App
3. Learn Basics of GIT
4. Extending our App
5. Deploy the APP to Heroku

## PART 2:
1. Use AT API’s to incorporate with the app
	a. Using SMS API
	b. Using AIRTIME API
	c. Using Payments API
	d. Using VOICE API

# 1. Introduction to Python
Python is a readable, dynamic, pleasant, flexible, fast and powerful high level programming language.

I suggest looking at the resources below for refresher courses.
    • xxx
    • xxx

Uses of Python Programming Language
    • Web Development
    • Scripting
    • Data Science – including machine learning, data analysis and data visualization

If you believe you can follow along, then dive in with me, I am just as excited as you are right now.

## Installing Python 3 and venv
Verify that python 3 is installed on your system by typing:

```
python3 -V

```

The output should look like this:

```
Python 3.6.6

```

To install the python3-venv package that provides the venv module which is the recommended module since python 3.6, run the following command:

```
sudo apt install python3-venv

```

Once the module is installed we are ready to create a virtual environment for our application.

Creating Virtual Environment
Start by navigating to the directory where you would like to store your Python 3 virtual environments a directory where your user has read and write permissions.

Create a new directory and navigate into it:

```
mkdir my_flask_app
cd my_flask_app

```

Once inside the directory, run the following command to create your new virtual environment:

```
python3 -m venv venv

```
This creates a directory called venv, which contains a copy of the Python binary, the Pip package manager, the standard Python library and other supporting files. You can use any name you want for the virtual environment.

To start using this virtual environment, you need to activate it by running this script:

```
source venv/bin/activate

```

Once activated, the virtual environment’s bin directory will be added at the beginning of the $PATH variable. Also your shell’s prompt will change and it will show the name of the virtual environment you’re currently using. In our case that is venv:

### Install dependencies

```
pip install -r requirements.txt

```
# Building The Flask App
Flask is a python micro-framework that is used to create Web Applications among others.



### Installing Flask
Now that the virtual environment is activated, you can use the Python package manager pip to install Flask:

```
pip install Flask

```

Within the virtual environment, you can use the command pip instead of pip3 and python instead of python3.

Verify the installation with the following command which will print the Flask version:

```
python -m Flask --version

```

You might see something similar to this:
```
Flask 1.0.2
Python 3.6.6 (default, Sep 12 2018, 18:26:19) 
[GCC 8.0.1 20180414 (experimental) [trunk revision 259383]]

```

Your Flask version may differ from the version shown here.

# 2. Creating a Minimal Flask Application
In this guide, we will create a simple hello world application which will just display the text “Hello World!”.

Open your text editor or Python IDE and create the following file:

~/my_flask_app/app.py

```
from flask import Flask
#import the Flask class

app = Flask(__name__)
#create an instance of the Flask class

@app.route('/')
#use the route() decorator to register the hello_world function for the / route

def hello_world():
    return 'Hello World!'
#route is requested, hello_world is called and the message “Hello World!” is returned to the client

```

Save the file as app.py and go back to your terminal window.

# 5. Testing the Development Server
We’ll use the flask command to run the application but before that we need to tell Flask how to load the application by specifying the FLASK_APP environment variable:

```
export FLASK_APP=app
flask run

```

The command above will launch the development built-in server.


The output will look something like the following:

```
* Serving Flask app "app"
* Environment: production
   WARNING: Do not use the development server in a production environment.
   Use a production WSGI server instead.
* Debug mode: off
* Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)

```

If you installed Flask on a virtual machine and you want to access Flask development server then you can make the server publicly available by appending --host=0.0.0.0 to the flask run command.

Open http://127.0.0.1:5000 in your web browser and you will be presented with the “Hello World!” message.

To stop the development server type CTRL-C in your terminal.

# 6. Deactivating the Virtual Environment
Once you are done with your work, deactivate the environment, by typing deactivate and you will return to your normal shell.

```
deactivate

```

## Introduction to GIT

GIT is a version control system. It is like Facebook for developers. ;-)

https://www.atlassian.com/git/tutorials

Verify that git is installed on your system by typing:

```
git --version

```

The output should look like this:

```
git x.x.x.x

```


Fork the repo to your computer  or folder you created.

[Fork me](https://github.com/abaeakili/at-mombasa)

Navigate to your directory and use the code below:

```
git clone  https://github.com/abaeakili/at-mombasa

```

Run the app

```
python app.py

```

Visit http://127.0.0.1:5000/ to view the site

## Deploy the APP to Heroku




### Conclusion

With this tutorial, I believe you have been able to use Python, install and create a virtual environment and install Flask, build a simple app send your files to GitHub, and finally be able to deploy your app on Heroku. 

Many thanks to Rahma Halane for Heroku Deployment Presentation, Fatima Muhsin for GITHUB Presentation, Aly Salim as the lead logistics and organizer, Daniel Otieno for the Flask Application and Introduction to Flask App, Kiplimo Kemboi for a great presentation on Python Programming language, all the attendants for joining us and the wonderful Team from Africa’s Talking (Liz and ..) for making this worth our precious time. We all benefited in so many ways.

I live at the intersection of Tech and Innovation. I enjoy a good laugh and warm coffee.

[Follow me on twitter:] @abaeakili
[Read my blogs:] bit.ly/abaeakili
[Check my GitHub:] github.com/abaeakili


Learnt the basics of Python, GIT, Flask, and Deployment of this APP on Heroku.

Follow Updates on Twitter #WeLoveNerds, @SwahiliBox, @africastalking and my handle @abaeakili
