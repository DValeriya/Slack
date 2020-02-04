## How to set up a server on Linux
***
### Creating virtual enviroment
   1. Git clone project:
        
         `$ git clone git@github.com:DValeriya/Slack.git`
   
   2. Go to the project directory. Once inside the directory, run the following command to create your new virtual environment ([more details](https://linuxize.com/post/how-to-install-flask-on-ubuntu-18-04/)):
 
        `$ python3 -m venv venv`
        
   3. To start using this virtual environment, you need to activate it by running the activate script:
   
        `$ source venv/bin/activate`
        
### Installing Flask
   Now that the virtual environment is activated, you can use the Python package manager pip to install Flask:
   
       (venv) $ pip install Flask
       
---

### Dependencies
You must install following dependencies:
        
        (venv) $ pip install flask  
        (venv) $ pip install flask-sqlalchemy
        (venv) $ pip install psycopg2-binary
        (venv) $ pip install slackeventsapi
        (venv) $ pip install slackclient
        (venv) $ pip install requets
 
### Environment variables
Set environment variables like below:
        
        (venv) $ export DB_USERNAME=" "
        (venv) $ export DB_NAME=" "
        (venv) $ export DB_PASSWORD=" "
        (venv) $ export DB_PORT=" "
        (venv) $ export DB_HOST=" "
        (venv) $ export SLACK_SIGNING_SECRET=" "
        (venv) $ export SLACK_APP_ID=" "
        (venv) $ export SLACK_BOT_SCOPE=" "
        (venv) $ export SLACK_CLIENT_SECRET=" "
        (venv) $ export SLACK_ACCESS_TOKEN=" "
        (venv) $ export SLACK_CLIENT_ID=" "
        
---

### Testing the Development Server
        
   We’ll use the flask command to run the application. The command below will launch the embedded development server:

        (venv) $ flask run

