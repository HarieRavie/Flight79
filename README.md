# Flight79
# Created a Flight Project inspired from ayush kumar flight project and thanks to him

# HOW TO INSTALL:

Install Python version more than 3.9+

# Create virtual environment and activate py -m venv "env name" and "env name"\Scripts\activate

# Run Required Modules using
" py -m pip install -r requirements.txt "

It will install required files
"Django
reportlab
xhtml2pdf
tqdm
gunicorn

# Check Django Installation: "django-admin"

# Go to required file path of django and connect to database using
"py manage.py makemigrations" "py manage.py migrate"

# Execution: "py manage.py runserver"

# Changes Affected:
* Created Account.html in template folder

* Created Account.css in Static/CSS folder
Set URL path path("Flight/account", Views.account_view, name="account"), in url.py page

* Added function name account_view in Views.py
def account_view(request): if request.user.is_authenticated: return render(request, 'flight/account.html',{'page': 'account'})

* Added Active functionality for My Account in layout.html

