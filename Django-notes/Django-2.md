# Django Template Language
* its use for make webpages dynamic
* by the help of templates we can create dynamic content for every user.

#### seprate folder for html/css
* we crate a seprate folder for html/css by any name
* My_hatml-->home.html-->heyy {name}

#### setup html/css path
* ``go to your project setting file  
    ``
    --->
    ``    DIRS:[os.path.join(BASE_DIR,'folder name in which you have html file)]``  -----> `` now change your view file for dynamic page ``
    ```
     return render(request,'home.html',{'name':'Pradyumn'})
     {}---> for database part
    ```
## Use of jinja
* basically jinja is use for extend the one html page functions to another html page

* in body part of base.html
```
{% block content %}

{% endblock %}

```
* 
```
{% extends base.html %}
{% block content %}

<h1>kjskjcc<h1>

{% endblock %}

```
