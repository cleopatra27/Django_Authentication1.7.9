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
    
and your done...should work just fine....you can always edit the html to make the login and sigup pages your own.
