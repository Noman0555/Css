# On click change pictures 
1st repository 
Author = Noman
<!DOCTYPE html>
<html>
<head>
    <title>Change Pictures</title>
    <script>
        function changeImage() {
            var imgElement = document.getElementById("myImage");
            var currentImage = imgElement.src;

            // Define the image URLs
            var image1 = "image1.jpg";
            var image2 = "image2.jpg";

            // Check the current image and switch to the other one
            if (currentImage.endsWith(image1)) {
                imgElement.src = image2;
            } else {
                imgElement.src = image1;
            }
        }
    </script>
</head>
<body>
    <h1>Change Pictures Example</h1>
    <img id="myImage" src="image1.jpg" alt="Image 1">
    <button onclick="changeImage()">Change Picture</button>
</body>
</html>
