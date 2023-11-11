# اليوم الاول لتدريب اطار Django

> لتنزيل الاطار نحتاج 
عمل الاوامر الاتيه

`pip install django`

> لانشاء مشروع 

`django startproject coca`

#### لاضافة تطبيق 
```
cd coca
python manage.py startapp hr
```

** لعمل hello word view **

> قم باضافة هذا الكود الاتي: 

> views.py
```
from django.http import HttpResponse
def index(request):
    return HttpResponse('Hello, World!')
```
> urls.py
```
from django.urls import include, path

urlpatterns = [
    path("index/", include("hr.urls")),
    path("admin/", admin.site.urls),
]
```

> اوامر اخرى
```
python manage.py makemigrations
python manage.py migrate
```




