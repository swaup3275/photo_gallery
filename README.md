PHOTO GALLERY BUILT USING DJANGO
=================================
===================================

django-smh_gallery
==================

A simple photo gallery app for the Django web framework.

Features
--------
*   __Gallery view__. A grid of thumbnailed images.
*   __Image view__. Displays the image, title, date, description.
*   __Management__ of galleries and images through the Django admin.


Technologies used
-----------------
*   [Python][1]: programming language.
*   [Django][2]: web framework.
*   [Bootstrap][3]: front-end framework.
*   [Foundation][4]: for its clearing widget (full screen carousel).
*   [Django-thumbs][7]: a thumbnailing app for Django.

As a django app
-------------------------
Deploy the folder smh_gallery as if it were another Django app and include the app in your settings.py.
any doubt check example provided in the myapp folder.


As a web application
-------------------------

### First steps, the hard part ###

Make a directory (i.e. web).

This application uses a database. By default sqlite engine is used.

Open a console and go to the root project folder "django-smh_gallery".
Synchronize/create the database. Type:
`python manage.py syncdb`
It will create the database and will ask you for the admin credentials that will be used in the future.

Run the testing server. Type:
`python manage.py runserver`

You should have the testing web server running, so if you try to open the http://localhost:8000 web, the home page appears.

### Directory tree ###
*   web
    *   django-smh_gallery
        *   deploy - contains sample files used when deploying on apache server.
        *   myapp - base application folder.
            *   settings.py - the configuration file.
        *   smh_gallery - django gallerry app.
    *   media - where the pictures you upload are stored.
    *   static - where app static files are stored once ``.


### Adding a gallery ###

1.  Open the webpage http://localhost:8000/admin/ and sign in with the credentials you set when your synchronized the database. You should see the Django administration page.
2.  Press "Add" on the Galleries row on the Smh_Gallery section.
3.  As name, write "my gallery", the description is up to you.
4.  you see a table with the added gallery. the second  colm thats the name your gallery will be identified with.
5.  the "My Gallery" link now takes you to an empty gallery.



