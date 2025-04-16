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
   - post_share view => to share posts via email.
   - Django forms to share posts and send email recommendations via Simple Mail Transfer Protocol (SMTP)