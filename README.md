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