# Ex.06 Book Front Cover Page Design
# Date:12/12/2025
# AIM:
To design a book front cover page using HTML and CSS.

# DESIGN STEPS:
## Step 1:
Create a Django Admin project.

## Step 2:
Create an app in the Django interface.

## Step 3:
Create a folder named 'static' in the app folder.

## Step 4:
Create a new HTML file in the static folder.

## Step 5:
Write the HTML code with relevant CSS properties.

## Step 6:
Choose the appropriate style and color scheme.

## Step 7:
Insert the images in their appropriate places.

## Step 8:
Publish the website in the LocalHost.

# PROGRAM:
views.py

from django.shortcuts import render

def book_cover(request):
    return render(request, 'book_cover.html')

urls.py

from django import views
from django.contrib import admin
from django.urls import path

urlpatterns = [
    path('admin/', admin.site.urls),
    path('', views.book_cover, name='cover'),
]

html code:
'''
{% load static %}
<html><!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>BOOK COVER</title>
    <style>

        body {
            margin: 0;
            padding: 0;
            background: antiquewhite;
            justify-content: center;
            align-items: center;
            font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
            height: 100vh;
            display: flex;
            
        }

        .cover {
            width: 420px;
            height: 620px;
            background-image: url('sunset.jpg.png');
            background-size: cover;
            background-position: center;
            border: 4px solid rgb(203, 168, 133);
            position: relative;
            box-shadow: 0 25px 40px black;
            padding: 20px;
            color: #1b3b3a;
        }

        .title {
            text-align: center;
            margin-top: 20px;
            font-size: 32px;
            font-weight: bold;
            letter-spacing: 2px;
            color: burlywood;
        }

        .subtitle {
            text-align: center;
            margin-top: 5px;
            font-size: 16px;
            color: beige;
        }

        .edition {
            font-size: 14px;
            margin-top: 40px;
            margin-left: 30px;
            border-bottom: 2px solid rgba(0,0,0,0.4);
            display: inline-block;
            padding-bottom: 4px;
        }

        .author {
            position: absolute;
            bottom: 60px;
            right: 40px;
            font-size: 25px;
            letter-spacing: 2px;
            background: bisque;
            padding: 4px 10px;
            border-radius: 6px;
        }

        .author-photo {
            position: absolute;
            bottom: 40px;
            left: 40px;
            width: 70px;
            height: 75px;
            border-radius: 50%;
            object-fit: cover;
            border: 2px solid blanchedalmond;
        }
    </style>
</head>

<body>

    <div class="cover">

        <div class="title">VOICE OF THE SUNSET</div>

        <div class="subtitle">Echoes carried by the Falling Sun</div>

        <div class="edition">TEMPORARY EDITION</div>

        <div class="author">NOT HITLER</div>

        <img src="NOT HITLER.png"class="author-photo" alt="Author Photo">

    </div>

</body>
</html>
'''
# OUTPUT:
<img width="1914" height="968" alt="Screenshot 2025-12-12 163219" src="https://github.com/user-attachments/assets/b5aca961-96ff-402a-aa2a-57a88468973e" />


# RESULT:
The program for designing book front cover page using HTML and CSS is completed successfully.
