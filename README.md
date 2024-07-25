# SOCIAL_WEBSITE

1. ver la version de `python --version`

2. selecionar la version de python se usa Ctrl + shift + P  y se selecciona Python: Select Interprete y se escoje la version que se desea trabajar.

3. crear el entorno virtual: `python -m venv venv`

4. pactivar el entorno virtual en windows `.\venv\Scripts\activate` y en unix o MAcOS es `source tutorial-env/bin/activate` 

5. instalar Django es `pip install django`

6.  ver las dependencias instaladas `pip freeze` si se desea crear el requirements.txt que espara cargar la dependencias se utiliza `pip freeze > requirements.txt` y para cargarlo se utiliza `pip install -r requirements.txt`.

7. la construccion del proyecto `django-admin startproject <nombre-proyecto>`

8. crear la migracion de la base de datos se dirige a la carpeta mysite y luego se el codigo `python manage.py migrate`

9. se usa el servidor web de python `python manage.py runserver`

10. se crea la app con `python manage.py startapp blog`

11. se aplica la migración `python manage.py makemigrations blog`

12. cuando se quiere saber que sentencia va a crear django para actuar con la base de datos `python manage.py sqlmigrate blog 0001` 0001 es el numero de la migración

13. para migrarlo `python manage.py migrate` 

[Django 4 by example (4th Edition) github](https://github.com/PacktPublishing/Django-4-by-example)

[Django 4 by example (4th Edition) book](https://books.google.es/books?id=GLaEEAAAQBAJ&pg=PA171&hl=es&source=gbs_selected_pages&cad=1#v=onepage&q&f=false)


### Prueba de cambio de contraseña

se utiliza `EMAIL_BACKEND = 'django.core.mail.backends.console.EmailBackend'` para simular el envio de un correo

envia el siguiente testo a la terminal para cambiar la contraseña

```bash
Content-Type: text/plain; charset="utf-8"
MIME-Version: 1.0
Content-Transfer-Encoding: 7bit
Subject: Password reset on 127.0.0.1:8000
From: webmaster@localhost
To: celioso1@hotmail.com
Date: Fri, 19 Jul 2024 22:54:02 -0000
Message-ID: <172142964276.17200.7346351970624961279@LaptopCelis>

Someone asked for password reset for email celioso1@hotmail.com. Follow the link below:
http://127.0.0.1:8000/account/password-reset/Mg/cafb22-bf8f3c88048d2f29c863cf5bc3b47138/
Your username, in case you've forgotten: pildoras
-------------------------------------------------------------------------------
```

### pillow
pillow es para trabajar con imagenes `pip install pillow`

[pillow](https://pypi.org/project/pillow/)
[Documentacion](https://pillow.readthedocs.io/en/stable/)

## Implementacion de autenticacion con redes sociales

**python-social-auth**

`pip install git+https://github.com/python-social-auth/social-app-django.git@20fabcd7bd9a8a41910bc5c8ed1bd6ef2263b328`

para el  cambio de hosts se ingresa a cmd como admin

```bash
Microsoft Windows [Versión 10.0.22631.3880]
(c) Microsoft Corporation. Todos los derechos reservados.

C:\Windows\System32>cd etc
El sistema no puede encontrar la ruta especificada.

C:\Windows\System32>cd drivers

C:\Windows\System32\drivers>cd etc

C:\Windows\System32\drivers\etc>notepad hosts

C:\Windows\System32\drivers\etc>
```
he ingresamos la siguiente direccion al final `127.0.0.1 mysite.com`

ya s epuede ingresar al link `http://mysite.com:8000/account/login/`

### Instalar django Extension

`pip install git+https://github.com/django-extensions/django-extensions.git@25a41d8a3ecb24c009c5f4cac6010a091a3c91c8`

luego `pip install werkzeug`

### RunServerPlus

`pip install pyOpenSSL`

iniciar el servidor: python manage.py runserver_plus --cert-file cert.crt

https://developers.facebook.com/app

### apuntalando el contenido en tu web
crear nuevo proyecto: `python manage.py startapp images`

### Para probar metodos 

```bash
(venv) PS C:\Users\celio\OneDrive\Escritorio\programación\practica-django\SOCIAL_WEBSITE\bookmarks>      python manage.py shell
Python 3.12.2 (tags/v3.12.2:6abddd9, Feb  6 2024, 21:26:36) [MSC v.1937 64 bit (AMD64)] on win32
Type "help", "copyright", "credits" or "license" for more information.
(InteractiveConsole)
>>> from django.utils.text import slugify
>>> slugify("Hola me llamo django")
'hola-me-llamo-django'

```
### Descargar imagenes con una URL

Con esto se utiliza para descargar imagenes desde una url
`pip install requests`

[django login social base](https://github.com/pildorasdeprogramacion/django-login-social-base)

[Prueba de Bookmark](https://127.0.0.1:8000/images/create/?title=%20Django%20and%20Duke&url=https://upload.wikimedia.org/wikipedia/commons/8/85/Django_Reinhardt_and_Duke_Ellington_%28Gottlieb%29.jpg)