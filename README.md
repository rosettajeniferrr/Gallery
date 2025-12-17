# Ex.06 Design of Interactive Image Gallery
# Date:15-12-25
# AIM:
To design a web application for an inteactive image gallery with minimum five images.

# DESIGN STEPS:
## Step 1:
Clone the github repository and create Django admin interface.

## Step 2:
Change settings.py file to allow request from all hosts.

## Step 3:
Use CSS for positioning and styling.

## Step 4:
Write JavaScript program for implementing interactivity.

## Step 5:
Validate the HTML and CSS code.

## Step 6:
Publish the website in the given URL.

# PROGRAM :
gallery.html
```
{% load static %}
<html>
<head>
    <title>Image Gallery</title>
    <link rel="stylesheet" href="{% static 'CSS.css' %}">
</head>

<body>
    <center>

<h2>Image Gallery</h2>
<div class="row">
    <img src="{% static 'image1.jpg' %}" width="400" height="300" onclick="openImg(this)">
    <img src="{% static 'image2.jpg' %}" width="400" height="300" onclick="openImg(this)">
    <img src="{% static 'image3.jpg' %}" width="400" height="300" onclick="openImg(this)">
</div>

<div class="row">
<img src="{% static 'image4.jpg' %}" width="400" height="300" onclick="openImg(this)">
<img src="{% static 'image5.jpg' %}" width="400" height="300" onclick="openImg(this)">
</div>

<div id="popup">
    <span id="close" onclick="closeImg()">&times;</span>
    <img id="popupImg">
</div>

<script>
function openImg(img){
    document.getElementById("popup").style.display = "flex";
    document.getElementById("popupImg").src = img.src;
}

function closeImg(){
    document.getElementById("popup").style.display = "none";
}
</script>

</center>
</body>
</html>


# OUTPUT:
# RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
