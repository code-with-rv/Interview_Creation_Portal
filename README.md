# Scaler-Task Submission
### Interview Creation Portal [(Link)](https://scaler-task.herokuapp.com/)

## Functionalities
* An interview creation page where the admin can create an interview by selecting participants, start time and end time. (also implemented basic validations using Django messages)
* An interviews list page where admin can see all the upcoming interviews.
* An interview edit page where admin can edit the created interview with the same validations as on the creation page.
* Email notification to participants on interview creation/rescheduling
* Option to upload resume 

## Database Schema 
<img src="https://raw.githubusercontent.com/kushagra219/Scaler-Task/main/assets/my_project_subsystem.png">

## Technologies Used
* Django - 3.2.9 
* Python - 3.8.5
* Database - sqlite3(development), postgresql(heroku)
* IDE - VS Code

## Getting Started
* Clone this repository.
* Set up a python virtual environment and activate it in your terminal. (Refer - <a>https://docs.python.org/3/tutorial/venv.html</a>)
* Create a `.env` file in the project root with the following variables (required by `interview_portal/settings.py`):
    ~~~
        SECRET_KEY=your-django-secret-key
        EMAIL_HOST_USER=your-gmail-address
        EMAIL_HOST_PASSWORD=your-gmail-app-password
    ~~~
* Open the repo in terminal and run the following commands - 
    ~~~ 
        pip install -r requirements.txt
    ~~~
    ~~~ 
        python manage.py makemigrations
    ~~~ 
    ~~~ 
        python manage.py migrate
    ~~~
    ~~~ 
        python manage.py runserver
    ~~~
* Open http://127.0.0.1:8000/ in your browser, login and explore 

## References
* https://docs.djangoproject.com/en/3.2/
* https://www.analyticsvidhya.com/blog/2020/10/step-by-step-guide-for-deploying-a-django-application-using-heroku-for-free/
