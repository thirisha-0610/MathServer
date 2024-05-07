# Ex.05 Design a Website for Server Side Processing
## Date: 19/04/2024

## AIM:
To design a website to find surface area of a Right Cylinder in server side.

## FORMULA:
Surface Area = 2Πrh + 2Πr<sup>2</sup>
<br>r --> Radius of Right Cylinder
<br>h --> Height of Right Cylinder

## DESIGN STEPS:

### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Create python programs for views and urls to perform server side processing.

### Step 5:
Create a HTML file to implement form based input and output.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
<!DOCTYPE html>
<html>
<head>
<title>Surface Area Of Right Cylinder</title>
<style type="text/css">
body
{
    background-color:pink;
}
.edge
{
    width: 1440px;
    margin-left: auto;
    margin-right: auto;
    padding-top: 100px;
}
.box
{
    display:block;
    border: ridge black;
    width: 900px;
    min-height: 500px;
    font-size: 20px;
    background-color:lightblue;
}
.my
{
    color:red;
    text-align: center;
    margin-top: 8px;
    margin-bottom: 9px;
}
.my1
{
    color:red;
    text-align: center;
    margin-top: 7px;
    margin-bottom: 6px;
    box-sizing: 20px;
}
h1
{
    color:black;
    text-align: center;
    padding-top: 20px;
}
</style>
</head>
<body>
    <div class="edge" align="center">
        <div class="box">
            <h1>SURFACE AREA OF A RIGHT CYLINDER</h1>
            <h2> THIRISHA A  (212223040228)</h2>
            <br>
            <br>
            <div class="my">
                <b>RADIUS : </b> <input type="text" name="Radius"></input> (in m)<br/>
                <br>
            </div>
            <div class="my">
                <b>HEIGHT : </b> <input type="text" name="Height"></input> (in m)<br/>
                <br>
            </div>
            <div class="my1">
                <input type="button" value="CALCULATE" onclick="calculateArea()"></input><br/>
                <br>
            </div>
            <div class="my">
                <b>AREA : </b> <input type="text" name="area"></input> m<sup>2</sup><br/>
            </div>
        </div>
    </div>
    <script type="text/javascript">
        function calculateArea()
        {
            var radius = parseFloat(document.getElementsByName("Radius")[0].value);
            var height = parseFloat(document.getElementsByName("Height")[0].value);
            var area = 2 * Math.PI * radius * (radius + height);
            document.getElementsByName("area")[0].value = area.toFixed(2);
        }
    </script>
</body>
</html>
```

## SERVER SIDE PROCESSING:

![Screenshot 2024-05-07 152216](https://github.com/thirisha-0610/MathServer/assets/149347494/d8f84650-b007-4dd4-a3bc-471dd934af8b)

## HOMEPAGE:
![Screenshot 2024-05-07 152135](https://github.com/thirisha-0610/MathServer/assets/149347494/5af79499-1438-4769-a569-2872b4667788)


## RESULT:
The program for performing server side processing is completed successfully.
