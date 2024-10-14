# Basic Poll App

## Writing your first Django app, part 1

1. Creating a project
1. The development server
1. Creating the Polls app
1. Write your first view

### Key Points

1. Create your project an app
2. Create a view function in views.py file.
3. Create a path in urls.py to map the view function to a URL.
4. Run the thing

```Shell
py .\manage.py runserver
```

## Writing your first Django app, part 2

1. Database setup
1. Creating models
1. Activating models
1. Playing with the API
1. Introducing the Django Admin
    1. Creating an admin user
    1. Start the development server
    1. Enter the admin site
    1. Make the poll app modifiable in the admin
    1. Explore the free admin functionality

### Key Points

1. Change your models (in models.py).
1. Run python manage.py makemigrations to create migrations for those changes
1. Run python manage.py migrate to apply those changes to the database.
1. Built in automated admin panel for managing models and data (add line to admin.py first)

```python
# Register your models here.
from .models import Question

admin.site.register(Question)
```

## Writing your first Django app, part 3

1. Overview
1. Writing more views
1. Write views that actually do something
   1. A shortcut: render()
1. Raising a 404 error
   1. A shortcut: get_object_or_404()
1. Use the template system
1. Removing hardcoded URLs in templates
1. Namespacing URL names

### Pt3 Key Points

- You can pass variables and parameters to views.py
- You can make paths leveraging variables in urls.py
- Use templates instead of hard coding into views.py
- you can create templates folder in the app directory and create an HTML file for each view function. 
- You need to have a folder for the app JUST in case due to djangos structure requirements, e.g. polls/templates/polls/index.html
- You should import render from django.shortcuts to use the render() shortcut function in views.py instead of template loader. it's less lines of code. more efficient.
- always namespace and loosely couple URLs in templates to avoid issues with other app template conflictions, and hard coded urls, e.g. < li >< a href="{% url 'polls:detail' question.id %}">{{ question.question_text }}< /a>< /li>
- 

## Resources

1. **Django Documentation:** https://docs.djangoproject.com/en/5.1/intro/