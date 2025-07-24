Icons in HTML are small images that show actions or items on a website, like a "home" button or a "search" symbol. They help people find things easily. To add icons in HTML, you can use an icon library like Font Awesome, Bootstrap Icons, Google Icons, and Image Icons.

1. Using Font Awesome Icons
Font Awesome is a popular icon library that provides scalable vector icons. To use Font Awesome, you need to include a CDN link to the library in your HTML document's <head> section. Then, you can use the appropriate class name associated with an inline element, such as the <i> tag, to display the required icon.

```
<head>
    <!-- Include Font Awesome icon library -->
    <link href=
"https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css" 
          rel="stylesheet" />
</head>
<body>
    <!-- Font Awesome Icon -->
    <i class="fas fa-home"></i>
</body>
```

Output

2. Using Bootstrap Icons
Bootstrap Icons are a collection of icons designed to be used with Bootstrap framework. To use Bootstrap Icons, include the Bootstrap Icons library using a CDN link in the <head> section of your HTML document. Then, use the <i> tag with the appropriate class name to display the icon.

```
<head>
    <!-- Include Bootstrap Icons library -->
    <link href=
"https://cdn.jsdelivr.net/npm/bootstrap-icons/font/bootstrap-icons.css" 
          rel="stylesheet" />
</head>
<body>
    <!-- Bootstrap Icon -->
    <i class="bi bi-house-fill"></i>
</body>
```

Output


3. Using Google Icons (Material Icons)
Google Icons, also known as Material Icons, provide a wide range of icons that follow Material Design guidelines. To use Google Icons, include the Google Icons library using a CDN link in the <head> section. Then, use the <span> tag with the class material-icons and specify the icon name.

```
<head>
    <!-- Include Google Icons library -->
    <link href=
"https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet" />
</head>
<body>
    <!-- Google Icon -->
    <span class="material-icons">home</span>
</body>
```

Output

4. Using Image as a Icons
You can also use image files as icons by utilizing the <img> tag . This method allows you to use custom images as icons. You can apply CSS to adjust the size of the icon as needed.

```
<img src="https://media.geeksforgeeks.org/wp-content/uploads/20240527124348/zi.png" 
         alt="home icon" style="width: 24px; height: 24px;" />
```

Output

How to Add GIF in HTML?
Last Updated : 11 Jun, 2025
GIFs (Graphics Interchange Format) are the popular image format that supports both animated and static images. Adding the GIFs to the HTML document enhances the visual appeal and the user interaction of the web pages. They are commonly used for loading animations, fun illustrations, or visual explanations.

There are multiple ways to add the GIFs to an HTML document:

Using the &lt;img&gt; Tag
The image tag is the standard way to embed the images in an HTML document, including GIFs. It is a self-closing that allows you to specify the source of the image, alternative text for accessibility, and other attributes like width and height.

Syntax

```
<img src="path-to-your-gif.gif" alt="Description of GIF" />
```

Example 1: This example shows the use of img tag for adding GIF.

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width,
          initial-scale=1.0">
    <title>GIF Example</title>
</head>
<body>
    <h2>Displaying a GeekforGeeks GIF using the
        <code>&lt;img&gt;</code> tag:
    </h2>
    <img src="gfg1.gif" alt="GeekforGeeks" width="400" height="300" />
</body>
</html>
```

Output

Using the CSS as a Background Image
Using the GIF as a background image via CSS is another effective method, especially for design the elements like buttons, divs, or entire sections of the webpage. This method can often used for the decorative purposes.

Syntax

```
<style>
    .class-name {
        background-image: url('path-to-your-gif.gif');
        background-size: cover;
        background-repeat: no-repeat;
    }
</style>
```

Example 2: This example shows the use of CSS to add the GIF as a background.

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width,
           initial-scale=1.0">
    <title>GIF as Background Image</title>
    <style>
        .gif-background {
            width: 500px;
            height: 300px;
            background-image: url('gfg1.gif');
            background-size: cover;
            background-repeat: no-repeat;
            border: 2px solid #ccc;
            text-align: center;
            line-height: 300px;
            color: black;
            font-size: 24px;
        }
    </style>
</head>
<body>
    <h2>Using a GIF as a background image:</h2>
    <div class="gif-background">
      This is a div with a GIF background</div>
</body>
</html>
```

Output

Using the JavaScript
JavaScript can provides the dynamic control over the DOM, making it possible to add the GIFs programmatically. This approach can be useful for the dynamically loading content based on the user interaction or specific conditions.

Syntax

```
let  img = document.createElement("img");
img.src = "path-to-your-gif.gif";
document.getElementById("target-element").appendChild(img);
```

Example 3: This example shows the use of JavaScript for adding GIF.

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport"
          content="width=device-width,
                   initial-scale=1.0">
    <title>GIF GeekforGeeks</title>
</head>
<body>
    <h2>Adding a GeekforGeeks using JavaScript:</h2>
    <div id="gif-container"></div>
    <script>
        let img = document.createElement("img");
        img.src = "blinkgfg.gif";
        img.alt = "A Dynamic GeekforGeeks GIF Example";
        img.width = 400;
        img.height = 200;
        document.getElementById("gif-container").appendChild(img);
    </script>
</body>
</html>
```

Output:

How to add video in HTML5 ?
Last Updated : 15 Jul, 2025
In This article, we will define how to add video content using a <video> element in the document. Before HTML5 came into existence, videos could only be played in a browser using a plugin like flash, but after the release of HTML5, adding a video to a web page is easy as adding an image. The HTML5 “video” element specifies a standard way to embed a video in a web page. There are three different formats that are commonly supported by web browsers – mp4, Ogg, and WebM. The table below lists the formats supported by different browsers:


Syntax: 

<video src="" controls></video>

Example:



```
<!DOCTYPE html>
<html>
​
<head>
    <title>
        Define a Video or move?
    </title>
</head>
​
<body>
    <h2>
        GeeksForGeeks
    </h2>
    <h2>
        HTML5: How to define 
        a Video or Movie?
    </h2>
​
    <p>
        Adding Video on my webpage
    <p>
        <video width="400" height="350" controls>
            <source src="myvid.mp4" type="video/mp4">
            <source src="myvid.ogg" type="video/ogg">
        </video>
</body>
​
</html>
```

Output:

Supported Browsers:
Google Chrome
Internet Explorer
Firefox
Opera
Safari

