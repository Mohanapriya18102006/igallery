# Ex.08 Design of Interactive Image Gallery
## Date:12-04-2025

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
    <title>INTERACTIVE IMAGE GALLERY</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: lightsalmon;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            flex-direction: column;
        }
        .gallery-container {
            max-width: 800px;
            margin: 20px auto;
            overflow: hidden;
            position: relative;
        }
        .gallery-slider {
            display: flex;
            transition: transform 0.5s ease;
        }
        .gallery-item {
            min-width: 100%;
            box-sizing: border-box;
        }
        .gallery-item img {
            width: 100%;
            display: block;
            border-radius: 10px;
        }
        .navigation {
            position: absolute;
            top: 50%;
            width: 100%;
            display: flex;
            justify-content: space-between;
            transform: translateY(-50%);
        }
        .navigation button {
            background-color: rgba(0, 0, 0, 0.5);
            color: white;
            border: none;
            padding: 10px;
            cursor: pointer;
            border-radius: 50%;
            font-size: 18px;
        }
        .navigation button:hover {
            background-color: rgba(0, 0, 0, 0.8);
        }
        h1 {
            text-align: center;
            margin-bottom: 20px;
        }
        footer {
            margin-top: 20px;
            font-size: 16px;
            color: #333;
        }
    </style>
</head>
<body>
    
    <div class="gallery-container">
        <div class="gallery-slider" id="slider">
            <div class="gallery-item">
                <img src="vijay.jpg" alt="VIJAY">
            </div>
            <div class="gallery-item">
                <img src="sec.jpg" alt="SAVEETHA ENGINEERING COLLEGE">
            </div>
            <div class="gallery-item">
                <img src="zuck.jpg" alt="MARK ZUCKERBURG">
            </div>
            <div class="gallery-item">
                <img src="tata.jpg" alt="RATAN TATA">
            </div>
            <div class="gallery-item">
                <img src="nakamoto.jpg" alt="SATOSHI NAKAMOTO">
            </div>
            <div class="gallery-item">
                <img src="musk.jpg" alt="ELON MUSK">
            </div>
            <div class="gallery-item">
                <img src="kalam.jpg" alt="DR. APJ ABDUL KALAM">
            </div>
        </div>
        <div class="navigation">
            <button id="prev">&#10094;</button>
            <button id="next">&#10095;</button>
        </div>
    </div>

    <footer>
        NANDA KISHOR 24011485
    </footer>

    <script>
        var slider = document.getElementById('slider');
        var prev = document.getElementById('prev');
        var next = document.getElementById('next');

        var currentIndex = 0;
        var totalItems = slider.children.length;

        function updateSlider() {
            slider.style.transform = 'translateX(-' + (currentIndex * 100) + '%)';
        }

        prev.onclick = function() {
            if (currentIndex > 0) {
                currentIndex--;
            } else {
                currentIndex = totalItems - 1;
            }
            updateSlider();
        };

        next.onclick = function() {
            if (currentIndex < totalItems - 1) {
                currentIndex++;
            } else {
                currentIndex = 0;
            }
            updateSlider();
        };
    </script>
</body>
</html>
```

## OUTPUT:

![Screenshot 2025-04-12 112404](https://github.com/user-attachments/assets/0b354dc4-4b01-4750-9d07-6df193eae80f)

![Screenshot 2025-04-12 112459](https://github.com/user-attachments/assets/456506e6-a866-4abb-9f0f-9d411e32c358)

![Screenshot 2025-04-12 112525](https://github.com/user-attachments/assets/2da416e6-ecf9-4a63-967c-9b41c66627d6)

![Screenshot 2025-04-12 112621](https://github.com/user-attachments/assets/8756c156-9f7b-446c-bd5e-f638ad9031a4)

![Screenshot 2025-04-12 112551](https://github.com/user-attachments/assets/1feddeba-d830-4e89-8d5c-fbad12211c46)

![Screenshot 2025-04-12 112721](https://github.com/user-attachments/assets/bfeec066-ac7e-47fa-86c9-f8939f383945)

![Screenshot 2025-04-12 112818](https://github.com/user-attachments/assets/0c2b12ed-41d4-41ad-af2c-c067d1e2d444)







## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
