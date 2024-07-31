Notes about the creation of a REST API with Django

````bash
# Este modulo nos permite crear un entorno virtual
pip install virtualenv
````

````bash
# Creamos el entorno virtual en un nuevo directiorio llamado 'venv'
python -m virtualenv venv

# Lo activamos
./venv/Scripts/activate
````

Ahora si podemos instalar todos los paquetes y dependencias del proyecto en un entorno virtual.

Instalamos **django** 
* Funcionalidades básicas de una aplicación django.
````bash
pip install django
````

Instalamos **djangorestframework** 
* Extendemos la funcionalidad de django con funcionalidades dedicadas a crear APIs

````
pip install djangorestframework
````

Iniciamos el proyecto de django
* Usamos el flag . para que cree el proyecto en la carpeta actual.

````
django-admin startproject projectName .
````

* Se creará una carpeta con el nombre dado y un archivo manage.py

Ejecutamos manage.py para iniciar el servidor

````bash
python manage.py runserver
````

Creamos una aplicación dentro de django

````bash
python manage.py startapp appName
````

Agregamos la aplicación y el módulo rest_framework en el archivo settings.py en la carpeta del proyecto django.

````python
# Application definition

INSTALLED_APPS = [
    'django.contrib.admin',
    'django.contrib.auth',
    'django.contrib.contenttypes',
    'django.contrib.sessions',
    'django.contrib.messages',
    'django.contrib.staticfiles',
    'appName',
    'rest_framework'
]
````