# django-docs
## create a folder python-django
create a virtual environment 
activate virtual environment
install python
install pip
install django "pip install Django"
create project "django-admin startproject pro1"
go to project folder "cd pro1"
create app in project "python3 manage.py startapp core"
open project in VS Code "code ."
create templates folder in app
create core folder in templates
create index.html file in core folder
open urls.py in project folder and add "include" with path and  "path('',include('core.urls')),"
create a new urls.py file in app and add 
"from django.urls import path
from . import views
urlpatterns = [
    path('',views.index,name="home"),
]"
create a function views.py file 
"def index(request):
    return render(request,' core/index.html')"

add app in settings.py file
add content in index.html file
run development server "pyhton3 manage.py reunserver"
