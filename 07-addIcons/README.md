Icons in HTML are small images that show actions or items on a website, like a "home" button or a "search" symbol. They help people find things easily. To add icons in HTML, you can use an icon library like Font Awesome, Bootstrap Icons, Google Icons, and Image Icons.

1. Using Font Awesome Icons
Font Awesome is a popular icon library that provides scalable vector icons. To use Font Awesome, you need to include a CDN link to the library in your HTML document's <head> section. Then, you can use the appropriate class name associated with an inline element, such as the <i> tag, to display the required icon.




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
Output

2. Using Bootstrap Icons
Bootstrap Icons are a collection of icons designed to be used with Bootstrap framework. To use Bootstrap Icons, include the Bootstrap Icons library using a CDN link in the <head> section of your HTML document. Then, use the <i> tag with the appropriate class name to display the icon.




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
Output


3. Using Google Icons (Material Icons)
Google Icons, also known as Material Icons, provide a wide range of icons that follow Material Design guidelines. To use Google Icons, include the Google Icons library using a CDN link in the <head> section. Then, use the <span> tag with the class material-icons and specify the icon name.




<head>
    <!-- Include Google Icons library -->
    <link href=
"https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet" />
</head>
<body>
    <!-- Google Icon -->
    <span class="material-icons">home</span>
</body>
Output

4. Using Image as a Icons
You can also use image files as icons by utilizing the <img> tag . This method allows you to use custom images as icons. You can apply CSS to adjust the size of the icon as needed.




<img src="https://media.geeksforgeeks.org/wp-content/uploads/20240527124348/zi.png" 
         alt="home icon" style="width: 24px; height: 24px;" />
Output


