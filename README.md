# Github Pages Tutorial

## Overview

In this tutorial, we'll learn ow to setup Github and develop a simple HTML and CSS template that is easy-to-learn, easy-to-implement and mobile responsive.

## First Lesson
### Setting Up Github Pages

1. Login to Github using your Github account
2. Create a new repository by clicking the plus button next to your profile picture and select new repository
3. Fill in all details (Description is optional, .gitignore is unnecessary for our case). MAKE SURE YOU HAVE A README AND HAVE SET THE REPOSITORY TO PUBLIC
4. Once the repository has been created, go over to the settings section of the repository. Keep scrolling down the settings until you find Github Pages. Currently, the source is set to none. Our code is going to be stored on the main (master) branch, so change the source from none to the branch name. Then change the folder location to '/' (root). Click save and your website should be on Github Pages. The link to your website will be 'your-username.github.io/repository-name'.

### Developing the Code
#### Developing the Navbar
##### HTML

In this lesson, we're going to be developing a simple navigation menu. Here's the HTML for the navigation menu - 

```HTML

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <link rel="stylesheet" type="text/css" href="style.css">
    <link href="https://fonts.googleapis.com/css2?family=Raleway:wght@300;400;500;600;700;800;900&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.4.1/css/all.css">
    <title>Education Model Template</title>
</head>
<body>
    <header>
        <nav>
            <ul>
                <li><a>Home</a></li>
                <li><a>About</a></li>
                <li><a>Blog</a></li>
                <li><a>Contacts</a></li>
            </ul>
        </nav>
    </header>
</body>
</html>

```

 Let's understand the code step by step. The file starts off with a DOCTYPE, which states that the file is a html file. We're then setting the language of the website to English. Inside our <head> (this is where you link CSS files, fonts, etc. to your website), we're first setting the character set to UTF-8. Next, we're link our CSS file, followed by a link to our Raleway font. After that, we're linking to an online CSS file from fontawesome.com. Then, we're setting the title of the HTML file to Education Model Template.
  
Inside the body, we have a container called header. Inside our header we have another container called nav. Inside that, we have an unordered list, inside of which are all our links for the navigation menu. An unordered list has no order, it's like your shopping list, whereas an ordered is like the steps in a cooking recipe. Inside our undordered lists, we have our list elements, inside of which is our links.

##### CSS

Here's the code for the CSS - 

```CSS

 * {
  margin:0;
  padding:0;
 }
 
 html {
  scroll-behavior:smooth;
 }

body {
  background:black;
  font-family:'Raleway', sans-serif;
}
 
 header {
  width:100%;
  height:100px;
  position:fixed;
  top:0;
  left:0;
  background:#fff;
 }

nav {
  width:100%;
  height:100%;
}

nav ul {
  height:100%;
  display:flex;
  gap:3em;
  margin-left:20%;
  align-items:center;
  font-size:1.25vw;
  font-weight:700;
  text-transform:uppercase;
  color:black;
  text-decoration:none;
  list-style:none;
}

nav a {
  text-decoration:none;
  color:black;
  transition: color 0.2s ease-in-out;
}

nav a:hover {
  color:#ef4d8c;
  transition: color 0.2s ease-in-out;
}

```

That might seem like a lot, but it can be broken down into small chunks. At the top of the CSS file, we're just removing any unneccesary margins annd padding. Margins and padding are the space around elements in a webpage. The differences between them are highlighted in this Youtube tutorial here - https://www.youtube.com/watch?v=EhbZGV2dqZ4. 

Next, we're setting the scroll-behaviour to smooth, just allowing scrolling to run smoothly on our website. We're then setting the background of our webpage to black (in case something weird happens) and our font-family to Raleway.

For our header, we're setting our width to be the same as the window itself followed by a height of 100px. We're then fixing the header to the top-left of our window. Fixing it to the top-right would have the same effect as the header takes the width of the window. Try it yourself! Lastly, we're setting the background of the header to white.

For our nav, we want it to take the shape of the header, that's why we set the width and height to 100%.

For our unordered list, we first set the height of it to be the same as the nav, and then gave it a display of flex. A display of flex will evenly space the elements inside the unordered list. We're making sure that there is a gap of 3em between each of the elements inside the unordered list. We're moving the unordered list to the right by 20%, vertically aligning all the elements inside our unordered list, setting a font-size of 1.25vw, a font-weight of 700 (the bigger the font-weight, the bolder the text), capitalising the text, setting a colour of black, removing all text-decoration (underlines, etc.) and removing all bullet points.

For our links (which are inside our unordered list), we're making sure that there is a text-decoration of none, a color of black. When the mouse is hovering over a link, then we want to change the colour to a pinkish colour with a transition of 0.2s.

## Lesson 2
### Documenting Code Using Markdown

Coming Soon.
