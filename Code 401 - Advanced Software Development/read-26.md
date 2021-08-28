# Readings: Intro to Django

- Django is a framework for Python that makes it easy to build web applications.

    ![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRyn8l24I-EGCC7jMiMsNi1ToY9IX06-KMb6g&usqp=CAU)

- Django was designed to help developers take applications from concept to completion as quickly as possible.

- battery included in the Django package is a great way to get started with Django.
  - Django includes dozens of extras you can use to handle common web development tasks. Django takes care of user authentication, content administration, site maps, RSS feeds, and many more tasks — right out of the box.

### URLs and views

- A clean, elegant URL scheme is an important detail in a high-quality Web application. Django encourages beautiful URL design and doesn’t put any cruft in URLs, like .php or .asp.

-To design URLs for an application, you create a Python module called a URLconf. Like a table of contents for your app, it contains a simple mapping between URL patterns and your views.

```
from django.urls import path

from . import views

urlpatterns = [
    path('bands/', views.band_listing, name='band-list'),
    path('bands/<int:band_id>/', views.band_detail, name='band-detail'),
    path('bands/search/', views.band_search, name='band-search'),
]
```

## How Django Works Behind the Scenes

- Django is a Python-based web framework used by millions of developers and billions of consumers through popular apps like Instagram. It is open source, meaning the code is available for free on Github and can be downloaded onto any developer’s computer and used alongside the official documentation.

ِAlmost all popular open source packages have some degree of funding involved, typically in one of three forms:

1. Corporate Sponsor - A group of engineers within a larger, for-profit company decide to open-source internal code. This is how React (Facebook) and Angular (Google) emerged. Typically engineers at the company are paid, in part, to work on open source though community involvement from developers outside of the core company occurs as well. While this structure has the stability of a wealthy benefactor, there can be confusion around the licensing aspects at times.

2. Solo - An individual developer initially creates code, open sources it, and retains default control. This is the case for VueJS, Tailwind CSS, and Laravel, among others. Typically the lead developer either raises contributions directly like Evan You of VueJS, offer add-on services like Spark for Laravel, or the founders provide highly-paid consulting services.

3. Non-profit - This was Django’s approach early on, in 2008, when the Django Software Foundation was formed to promote, support, and advance Django.