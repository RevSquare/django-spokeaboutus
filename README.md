django-spokeaboutus
===================

SpokeAboutUs is a django application to store and display short messages about
your service


Instalation
-----------

``pip install -e git+https://github.com/tomaszroszko/django-spokeaboutus.git#egg=django_spokeaboutus.git``

*settings.py*

```

INSTALED_APPS = (
    ...
    'spokeaboutus',
    ...
)
```

*urls.py*

```

urlpatterns = patterns('',
    ...
    url(r'^spoke-about-us/', include('spokeaboutus.urls')),
    ...
)
```

*run commands*

```
python manage.py syncdb
python manage.py migrate
```

