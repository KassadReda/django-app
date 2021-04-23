

## Configuration

### Virtual environment

You should better use a virtual environment to use this project so that you won't have too many packages installed.

&nbsp;

Ubuntu:

```console
create a new environment : python3 -m venv my_project/venv
activate venv : source my_project/venv/bin/activate
deactivate venv : deactivate
```

Windows:

```console
create a new environment : virtualenv --python C:\Path\To\Python\python.exe venv
activate venv : .\venv\Scripts\activate
deactivate venv : deactivate
```

&nbsp;

You can find you path for Python by using :

Ubuntu:

```console
which python
```

Windows:

```console
where python
```

(you may need to put python to your Path : <https://datatofish.com/add-python-to-windows-path/>)

&nbsp;

### Requirements

Once you are into your virtual environment you need to install every pip packages needed.

The requirements are:

```console
asgiref==3.3.0
certifi==2020.6.20
Django==3.1.3
django-crispy-forms==1.9.2
Pillow==8.0.1
pytz==2020.4
sqlparse==0.4.1
gunicorn
django-heroku
whitenoise
```

&nbsp;

You can use this command to install them quickly :

```console
pip install -r requirements.txt
```

&nbsp;

If you need to push more packages into the requirements file, then use :

```console
pip freeze > requirements.txt
```

&nbsp;

### Run project

Now that everything is ready, you can simply run your server on your local port :

```console
cd click_collect
python manage.py runserver
```

