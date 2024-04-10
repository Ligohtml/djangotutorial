# DJANGO TUTORIAL
https://cs50.harvard.edu/web/2020/notes/3/
### Install 
1)
```html
pip install django
```

2) Run ``` python -m django startproject PROJECT_NAME ``` to create a number of starter files for our project.  

3) Run ``` cd PROJECT_NAME ``` to navigate into your new project’s directory.  

4) Open the directory in your text editor of choice. You’ll notice that some files have been created for you. We won’t need to look at most of these for now, but there are three that will be very important from the start:  

- **manage.py** is what we use to execute commands on our terminal. We won’t have to edit it, but we’ll use it often.
- **settings.py** contains some important configuration settings for our new project. There are some default settings, but we may wish to change some of them from time to time.
- **urls.py** contains directions for where users should be routed after navigating to a certain URL.
  
Start the project by running ``` python manage.py runserver ```. This will open a development server, which you can access by visiting the URL provided. This development server is being run locally on your machine, meaning other people cannot access your website.  
This should bring you to a default landing page:  

5) Next, we’ll have to create an application. Django projects are split into one or more applications. Most of our projects will only require one application, but larger sites can make use of this ability to split a site into multiple apps.
To create an application, we run ``` python manage.py startapp APP_NAME ```. This will create some additional directories and files that will be useful shortly, including views.py.

6) Now, we have to install our new app. To do this, we go to settings.py, scroll down to the list of INSTALLED_APPS, and add the name of our new application to this list.
   
   <img width="407" alt="installed" src="https://github.com/Ligohtml/djangotutorial/assets/150527102/9523886a-140c-4115-9bb0-b6616ec0e92d">
