# Django_Authentication1.7.9
django login, signup, logout, forgot password forms and functunatity.

                                  WHAT NEXT??
Take the accounts app to your project.
update your INSTALLED APPS in your settings, add 'accounts',
add this line to your settings 
                     LOGIN_REDIRECT_URL = "index" (please change the 'index' to the name for your redirect url)
add the following line to your global url
                      url(r"^accounts/", include("accounts.urls", namespace="accounts")),                                       
                      url(r"^accounts/", include("django.contrib.auth.urls")),
                      
Add the following to your settings.py to allow email password reset
       EMAIL_BACKEND = "django.core.mail.backends.filebased.EmailBackend"
       EMAIL_FILE_PATH = os.path.join(BASE_DIR, "sent_emails")
    
and your done...should work just fine....you can always edit the html to make the login and sigup pages your own.
