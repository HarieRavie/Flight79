# Flight79
Created a Flight Project inspired from ayush kumar flight project and thanks to him

HOW TO INSTALL:

Install Python version more than 3.9+

Create virtual environment and activate 
py -m venv "env name" and "env name"\Scripts\activate

Run Required Modules using
" py -m pip install -r requirements.txt "
It will install required files 
"Django==3.1.2
reportlab==3.5.57
xhtml2pdf==0.2.5
tqdm==4.64.0
gunicorn==20.1.0"

Check Django Installation:
"django-admin"

then got to required file path of django and connect to database using
"py manage.py makemigrations"
"py manage.py migrate"

Execution:
"py manage.py runserver"

Changes Affected:
•	Created Account.html in template folder,
•	Created Account.css in Static/CSS folder,
•	Set URL path path("Flight/account", Views.account_view, name="account"), in url.py page
•	Added function name account_view in Views.py 
def account_view(request):
    if request.user.is_authenticated:
        return render(request, 'flight/account.html',{'page': 'account'})
•	Added Active functionality for My Account in layout.html
<li class="nav-item dropdown my-account {% if page == 'account' %}active{% endif %}">

