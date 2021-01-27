## 1. Creating a repository on github.
> git clone git@github.com:login/repository.git 
_______________________________________________

## 2. Installation Django
### 1. Creating venv
```
sudo pip install virtualenvwrapper
```
Add in .bashrc
>```
>export VIRTUALENVWRAPPER_PYTHON=/usr/bin/python3
>export WORKON_HOME=~/venv
>. /usr/local/bin/virtualenvwrapper.sh 
>```
```
exec bash
```
```
mkvirtualenv --python=/usr/bin/python3 name_venv

(name_venv) deactivate

workon name_venv

rmvirtualenv name_venv
```
*Built-in venv module*
>```
>python3 -m venv venv
>source venv/bin/activate
>```

### 2. Install Django
```
pip install Django
```
### 3. Start project
```
django-admin startproject project_name
cd project_name
python manage.py startapp app_name
```
>**Choice interpreter and add project folder to workspace**
```
python manage.py runserver
```
>**Add app in settings.py**
>```
>'app_name.apps.AppConfig',
>```
>Change language maybe
_____
## 3. Controller for the main page.
### 1. Creating urls.py in app folder.
______
## 4. Transferring a template to a project.
### 1. Creating static folder in proj_app and copy everything except *.html
### 2. Configuration settings.py
```
python manage.py collectstatic
```
### 3. Creating templates folder and insert app folder and crreate index.html
### 4. In project folder create folder templates and insert file base.html
```
python manage.py collectstatic
```
_______________________
## 4. Config mmodel.py
```
python manage.py makemigrations
python manage.py migrate 

```
__________________________
## 5. Admin.
### 1. Config settings.py and urls.py
```
python manage.py createsuperuser