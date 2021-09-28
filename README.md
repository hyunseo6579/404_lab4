# 404_lab4

Q1. https://github.com/hyunseo6579/404_lab4/

Q2. It shows default Django website that says "The install worked successfully! Congratulations!" and some other details.

Q3. root directory ('/') throws 404 error as the page is not set in mysite/urls.py, but /polls takes me to /polls/ which gives simple page that says "Hello, world. You're at the polls index."

Q4. Migration is needed to setup a new table in the database based on the edits we make in models.py. This also lets us manage our database in our django admin page.

Q5. On the admin page, I see basic database tables (Groups, Users) under Authetication and Authority and the custom tables (Choices, Questions) under Polls.
To make my custom models to appear in Django admin page, I need to set it up by writing admin.site.register([table name]) in admin.py.

Q6. The page says, "You're looking at question 38." In /results it says "You're looking at the results of question 38." In /vote it says "You're voting on question 38."
Putting in string instead of number throws 404 error. I can modify this by changing the path from '<int:question_id>/' to '<str:question_id>/'.

Q7. If I hardcode urls in the template, I can only use the template when I need it to call only that specific url. This ruins the whole purpose of creating a template since I cannot reuse the template.

Q8. Generic view lets us simplify writing views. Use it to create a simple webpage, but not when I want to make more customized view.
