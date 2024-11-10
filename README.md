# Ex-7: Interactive Image Gallery
## Date: 10-11-2024

## AIM:
To design a book front cover page using HTML and CSS.

## DESIGN STEPS:

### Step 1:
Create a Django Admin project.

### Step 2:
Create an app in the Django interface.

### Step 3:
Create a folder named 'static' in the app folder.

### Step 4:
Create a new HTML file in the static folder.

### Step 5:
Write the HTML code with relevant CSS properties.

### Step 6:
Choose the appropriate style and color scheme.

### Step 7:
Insert the images in their appropriate places.

### Step 8:
Publish the website in the LocalHost.

## PROGRAM:

### index.html

```
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Interactive Photo Gallery</title>
  <link rel="stylesheet" href="style.css">
</head>

<body>
  <h1>Interactive Photo Gallery</h1>
  <div id="image">Hover over an image below to display here.</div>

  <div class="gallery">
    <img class="preview" alt="chruch in citadel" src="https://images.pexels.com/photos/29139391/pexels-photo-29139391/free-photo-of-dome-of-palacio-de-bellas-artes-in-mexico-city.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" onmouseover="upDate(this)" onmouseout="unDo()">
    <img class="preview" alt="winter arc" src="https://images.pexels.com/photos/3122798/pexels-photo-3122798.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" onmouseover="upDate(this)" onmouseout="unDo()https://images.pexels.com/photos/3122798/pexels-photo-3122798.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1">
    <img class="preview" src="https://images.pexels.com/photos/29232927/pexels-photo-29232927/free-photo-of-young-woman-dancing-joyfully-in-a-flower-field.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" alt="stunning beauty" onmouseover="upDate(this)" onmouseout="unDo()">
    <img class="preview" alt="birds" src="https://images.pexels.com/photos/16878538/pexels-photo-16878538/free-photo-of-a-seagull-is-standing-in-the-grass-near-some-bushes.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" onmouseover="upDate(this)" onmouseout="unDo()">
    <img class="preview" alt="bathing dog" src="https://images.pexels.com/photos/8343333/pexels-photo-8343333.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" onmouseover="upDate(this)" onmouseout="unDo()">
    <img class="preview" src="https://images.pexels.com/photos/29156944/pexels-photo-29156944/free-photo-of-seljalandsfoss-waterfall-in-iceland-s-scenic-landscape.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" alt="waterfalls" onmouseover="upDate(this)" onmouseout="unDo()">
  </div>
  <script src="script.js"></script>
</body>

</html>
```

### gallery.css
```
body {
  margin: 2%;
  border: 1px solid black;
  background-color: #b3b3b3;
}
#image {
  line-height: 650px;
  width: 575px;
  height: 650px;
  border: 5px solid black;
  margin: 0 auto;
  background-color: #8e68ff;
  background-image: url("");
  background-repeat: no-repeat;
  color: #ffffff;
  text-align: center;
  background-size: 100%;
  margin-bottom: 25px;
  font-size: 150%;
}
.preview {
  width: 10%;
  margin-left: 17%;
  border: 10px solid black;
}
img {
  width: 95%;
}

```
### gallery.js
```
// Reference to the image container
const imageDiv = document.getElementById("image");
const originalImageUrl = ""; // Set this to the URL of your original image
const originalText = "Hover over an image below to display here."; // Original text

function upDate(previewPic) {
  // Change the background image to the source of the hovered image
  imageDiv.style.backgroundImage = `url('${previewPic.src}')`;

  // Update the text to the alt text of the hovered image
  imageDiv.innerHTML = previewPic.alt;
}

function unDo() {
  // Reset the background image to the original URL
  imageDiv.style.backgroundImage = `url('${originalImageUrl}')`; // Use the original image URL here

  // Change the text back to the original text
  imageDiv.innerHTML = originalText;
}

```

## WEBSITE URL

https://codepen.io/Ranjan-Virgo/pen/poMqoLK


## OUTPUT:

![Screenshot 2024-11-10 165432](https://github.com/user-attachments/assets/ae9209f0-4155-439a-b253-c25bbf538d00)

![Screenshot (7)](https://github.com/user-attachments/assets/32259839-0032-442c-b7b5-1b383f941a84)



## RESULT:
The program for designing book front cover page using HTML and CSS is completed successfully.
