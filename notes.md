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

Iniciamos el projecto de django
* Usamos el flag . para que cree el proyecto en la carpeta actual.

````
django-admin startproject projectName .
````

* Se creará una carpeta con el nombre dado y un archivo manage.py

Ejecutamos manage.py para iniciar el servidor

````bash
python manage.py runserver
````