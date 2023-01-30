# Design a Website for Server Side Processing

## AIM:
To design a website to perform mathematical calculations in server side.

## DESIGN STEPS:
Step 1:
Create a django project inside the pulled GitHub Repo.

Step 2:
Insdie the project create a app called mathapp using command "sudo python3 manage.py startapp mathapp".

Step 3:
Create a template folder inside mathapp and inside than create another folder called mathapp and inside that create a new file "area.html"

Step 4:
Add the html conents in the area.html.

Step 5:
Do the mathemical calculation in views.py and link the html tags.

Step 6:
Link the html file through views.py in urls.py.

Step 7:
Add mathapp to installed apps in setting.py and add necessary changes

## PROGRAM :

<!DOCTYPE html>
<html>
<head>
    <meta charset='utf-8'>
    <meta http-equiv='X-UA-Compatible' content='IE=edge'>
    <title>Area</title>
    <meta name='viewport' content='width=device-width, initial-scale=1'>
    <style>
        body{
            text-align: center;
            background-color: #ade8f4;
            color: #081c15;
        }
        div{
            display: block;
            background-color: #48cae4;
            text-align: center;
            border-radius: 20px;
            width: 500px;
            height: 200px;
            margin-left: auto;
            margin-right: auto;
        }
        form{
            padding-top: 25px;
        }
        input{
            text-align: center;
            border-radius: 20px;
            text-align: center;
            box-shadow: 1.5px 7px #00b4d8;
            background-color: #caf0f8;
        }
    </style>
</head>
<body>
    <h1>Area of Triangle</h1>
    <div>
        <form method="POST">
            {% csrf_token %}
            Base = <input type="text" name="base" value="{{b}}"> m <br/>
            <br/>
            Height = <input type="text" name="height" value="{{h}}"> m <br/>
            <br/>
            <input type="submit" value="Calculate"><br/>
            <br/>
            Area = <input type="text" name="area" value="{{area}}"> m<sup>2 </sup><br/>
        </form>
    </div>
</body>
</html>

## OUTPUT:

### Home Page:


## Result:

