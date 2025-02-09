

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Be My Valentine</title>
</head>
<body>
    <h1>Will you be my Valentine?</h1>
    
    <button onclick="showMessage('yes')">Yes</button>
    <button onclick="showMessage('no')">No</button>

    <div id="response"></div>
    <img id="image" src="" alt="">

    <script>
        function showMessage(answer) {
            let response = document.getElementById('response');
            let img = document.getElementById('image');
            
            if (answer === 'yes') {
                response.innerHTML = "Yay! You're my Valentine!";
                img.src = "images/1.our-photo.jpg";  // Path to your photo in the "images" folder
            } else {
                response.innerHTML = "Are you sure?";
                img.src = "images/2.broken-heart.jpg";  // Path to the broken heart image
            }
        }
    </script>
</body>
</html>
```

