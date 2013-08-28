wconsumer_github_connect
========================

Implements "Connect with GitHub" feature allowing user to sign in or sign up with his GitHub account. 

User flow is as follows:

1.  User clicks Connect with GitHub link in login form.
1.  Module authenticates user with GitHub and retrieves his GitHub account data.
1.  If there is a user registered in Drupal having same GitHub url ('html_url' field of GitHub /user response, looks like "http://github.com/username") then user is logged in with this account.
1.  If there is no such account then try to register user with his GitHub login and email.
1.  If registration fails (login or email already taken, etc) then redirect user to the register page and allow him to manually register a new account.
