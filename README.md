# Ex:07 Design of Interactive Image Gallery
## Date:24/12/2025

## AIM:
To design a web application for an inteactive image gallery with minimum five images.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for positioning and styling.

### Step 4:
Write JavaScript program for implementing interactivity.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
<html>
<head>
    <title>Interactive Image Gallery</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <h1> Image Gallery</h1>

    <div class="gallery-container">
        <img id="galleryImage" src="furniture.png" alt="Gallery Image">

        <div class="buttons">
            <button id="prevbutton">Previous</button>
            <button id="nextbutton">Next</button>
        </div>
    </div>


    <footer>
        <p>Designed & Developed by Dhanalakshmi C © 2025</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>
body {
    font-family: italic,serif;
    background-color: whitesmoke;
    text-align: center;
}

h1 {
    margin-top: 22px;
}

.gallery-container {
    width: 520px;
    margin: 32px auto;
    background: lightgoldenrodyellow;
    padding: 13px;
    border-radius: 12px;
    box-shadow: 0 0 10px rgba(0,0,0,0.2);
}

.gallery-container img {
    width: 100%;
    height: 320px;
    object-fit: cover;
    border-radius: 7px;
}

.buttons {
    margin-top: 16px;
}

button {
    padding: 12px 22px;
    font-size: 18px;
    margin: 7px;
    border: none;
    border-radius: 6px;
    background-color: antiquewhite;
    color: rgb(230, 130, 8);
    cursor: pointer;
}

button:hover {
    background-color:blue;
}
footer {
    margin-top: auto;
    background-color: #333;
    color: white;
    padding: 15px 0;
    font-size: 14px;
}
const images = [
    "robot.png",
    "nature.png",
    "space.png",
    
];

let currentIndex = 0;

const galleryImage = document.getElementById("galleryImage");
const nextBtn = document.getElementById("nextbutton");
const prevBtn = document.getElementById("prevbutton");

nextBtn.addEventListener("click", () => {
    currentIndex = (currentIndex + 1) % images.length;
    galleryImage.src = images[currentIndex];
});

prevBtn.addEventListener("click", () => {
    currentIndex = (currentIndex - 1 + images.length) % images.length;
    galleryImage.src = images[currentIndex];
});
```


## OUTPUT:
<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/2c81c0e1-bc19-4bb2-bdec-b14b2ef54a4a" />
<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/7b896db6-8be0-41a7-bb9a-4af0cce7b822" />
<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/dfc1421f-8e5c-42e9-b56b-5f7a4c76cb17" />
<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/e224eaa8-0805-465f-a915-eb55e762d2a2" />





## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
