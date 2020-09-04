## To run in local python virtual environment:<br/>

Create virtual environment inside of this directory or some else directory which is not inside of project. <br/>
But if you want to create virtual environment inside of project you should name it venv(I already add venv
to .gitignore no matter the directory of it. To create virtual environment the command should be :<br/>
if virtual environment exists by default:<br/>
python3 -m venv venv<br/>
if you create by hand:<br/>
virtualenv venv<br/>
then to activate:<br/>
for windows:<br/>
venv/Scripts/activate<br/>
for mac:<br/>
. venv/bin/activate<br/>

Then you should install packages in requirements if any new package was added to project :<br/>
pip install -r requirements.txt<br/>

Then the project is ready to go. To create or update database:<br/>
python manage.py makemigrations<br/>
python manage.py migrate<br/>
python manage.py runserver<br/>
if that does not work try with python3 like:<br/>
python3 manage.py makemigrations<br/>
python3 manage.py migrate<br/>
python3 manage.py runserver (sometimes virtualenv needs to specified version of python so if it does not work try python3.7)<br/>
In this case the backend will be served in 127.0.0.1:8000/<br/>
