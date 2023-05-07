# 3_Project_Flask

This code is a simple Flask web application that has three routes: /, /register, and /login. It imports Flask, render_template, request, redirect, and url_for modules.

The app object is initialized as a Flask instance. Three global variables name, email, and password are defined with a value of None.

The / route renders a template named index.html using the render_template function when the user visits the root URL.

The /register route accepts both GET and POST requests. If the request method is POST, the function retrieves the values entered by the user in the registration form for name, email, and password fields and stores them in the corresponding global variables. Then, it redirects the user to the login page using the redirect function and the url_for helper function. If the request method is GET, the function simply renders the register.html template.

The /login route also accepts both GET and POST requests. If the request method is POST, the function renders the welcome.html template, which displays a welcome message and the name entered by the user during the registration. If the request method is GET, the function renders the login.html template, which contains a form to enter the email and password. It also pre-populates the form with the email and password values stored in the global variables.

Finally, the if __name__ == '__main__' statement runs the Flask application in debug mode.
