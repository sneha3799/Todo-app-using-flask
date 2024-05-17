# Todo-app-using-flask
Created a basic Todo CRUD app using Flask, HTML and CSS.
Steps to deploy the application on AWS Beanstalk. 
1. Create an application and environment by going to AWS Beanstalk
2. Go to terminal in Mac and create a new directory for the flask app -> mkdir flaskapp
3. Switch to the new directory -> cd flaskapp
4. Create app.py
5. Execute the following cmd in terminal to create a virtual environment -> pip install virtualenv and python -m virtualenv env
6. Activate the virtual env -> source env/bin/activate
7. Install flask -> pip install flask
8. Find all the installed libraries/ dependencies -> python -m pip freeze
9. Copy and paste all the libraries/ dependencies in a new file named as requirements.txt
10. Make a subfolder named .ebextensions and a new file python.config which is the configuration file for deploying app on AWS Beanstalk
11. Create a file .ebignore and add your virtual environment name to it (in my case it's 'env')
12. Zip all the files and sub-folders ->  zip -r file.zip \.* * (it's important to zip it using this cmd else the hidden files and directories won't be included in the zip file if done through the traditional way)
13. You can view all the hidden files in the directory using ls -la

References
- https://www.youtube.com/watch?v=fGxY_Hji8_U
- https://medium.com/analytics-vidhya/deploying-a-flask-app-to-aws-elastic-beanstalk-f320033fda3c
- https://www.youtube.com/watch?v=iBeOvmt-tR0
