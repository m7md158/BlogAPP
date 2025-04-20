# chapter1
## Custome Admin file
   - blog.admin.py

### PublishedManager

# -----------------------------

# chapter2 
   - Canonical URLs Django => product -> product detail = get_absoulte_url 
   - slug
   - pagination 
      [Let’s review the new code we have added to the view:
         1. We instantiate the Paginator class with the number of objects to return per page. We will 
         display three posts per page.
         2. We retrieve the page GET HTTP parameter and store it in the page_number variable. This parameter contains the requested page number. If the page parameter is not in the GET parameters 
         of the request, we use the default value 1 to load the first page of results.
         3. We obtain the objects for the desired page by calling the page() method of Paginator. This 
         method returns a Page object that we store in the posts variable.
         4. We pass the posts object to the template.]
         

         
   - class based views
      - class based view اقل ف الكود بس فيه تعديل ف page.html -> 
            {% include "pagination.html" with page=page_obj %}

   - post_share view => to share posts via email.
      - Recommending posts by email We will allow users to share blog
         posts with others by sending post recommendations via email
         You will learn how to create forms in Django, handle data submission, and send emails with Django, enhancing your blog with a personal touch.
         To allow users to share posts via email, we will need to:
         1. Create a form for users to fill in their name, their email address, the recipient’s email address.
            Django comes with two base classes to build forms:
            • Form: This allows you to build standard forms by defining fields and validations.
            • ModelForm: This allows you to build forms tied to model instances. It provides all the functionalities of the base Form class, but form fields can be explicitly declared, or automatically 
            generated, from model fields. The form can be used to create or edit model instances.
         and optional comments
         2. Create a view in the views.py file that handles the posted data and sends the email
         3. Add a URL pattern for the new view in the urls.py file of the blog application
         4. Create a template to display the form

   - Sending emails with Django
      - We will add SMTP configuration settings to the project
      - python -m pip install python-decouple==3.8

   - Creating a comment system
      


   - Django forms to share posts and send email recommendations via Simple Mail Transfer Protocol (SMTP)

# -----------------------------------------

# chapter3

   - Implementing tagging with django-taggit
      python -m pip install django-taggit==5.0.1  -> installed_app

   - Retrieving posts by similarity
   - Creating custom template tags and filters