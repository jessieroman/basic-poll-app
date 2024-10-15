# Basic Poll App

## Writing your first Django app, part 1

1. Creating a project
1. The development server
1. Creating the Polls app
1. Write your first view

### Pt1 Key Points

- Create a Django project and app.
- Define a view function in views.py.
- Map the view to a URL in urls.py.
- Run the server: python manage.py runserver.

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

### Pt2 Key Points

- Define models in models.py.
- Run makemigrations to track changes and migrate to apply them.
- Register models in admin.py to manage via the admin panel:

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

- Use render() to simplify rendering templates.
- Replace hardcoded URLs in templates with {% url %}.
- Organize templates in polls/templates/polls/.
- Use get_object_or_404() for cleaner error handling.
- Namespace URLs to avoid conflicts between apps.

```html
<li><a href="{% url 'polls:detail' question.id %}">{{ question.question_text }}</a></li>
```

## Writing your first Django app, part 4

1. Write a minimal form
2. Use generic views: Less code is better
   1. Amend URLconf
   2. Amend views

### Pt4 Key Points

- Always use HttpResponseRedirect to avoid people resubmitting on back button.
- Use POST when updating data in web apps as a best practice.
- `{% csrf_token %} for Cross Site Request Forgery protection.


## Resources

1. **Django Documentation:** https://docs.djangoproject.com/en/5.1/intro/