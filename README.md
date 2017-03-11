# django-custom-user
Simple template for adding custom user model that provides all the functionality that standard model provides but uses email field as the main authentication field instead of username field.

# Steps:
1. Put `custom_user` folder to root folder of your django_app.
2. Alternatively change app name:
    * change folder name
    * In the `apps.py` change lines 4 and 5 respectively
3. Add `'custom_user'` to `INSTALLED_APPS`
4. Add this line `AUTH_USER_MODEL = 'custom_user.User'` to your `settings.py`
5. Run `python manage.py makemigrations custom_user`
6. Run `python manage.py migrate`
7. DONE
