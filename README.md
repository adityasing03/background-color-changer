<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Background Color Changer</title>
  <style>
    body {
      margin: 0;
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      font-family: sans-serif;
      transition: background-color 0.3s ease;
    }
    .container {
      text-align: center;
    }
    button {
      padding: 10px 20px;
      font-size: 16px;
      border: none;
      background-color: #007bff;
      color: white;
      border-radius: 5px;
      cursor: pointer;
    }
    button:hover {
      background-color: #0056b3;
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>Click to Change Background Color</h1>
    <button onclick="changeColor()">Change Color</button>
  </div>

  <script>
    function changeColor() {
      const colors = ['#f44336', '#2196f3', '#4caf50', '#ff9800', '#9c27b0'];
      const randomColor = colors[Math.floor(Math.random() * colors.length)];
      document.body.style.backgroundColor = randomColor;
    }
  </script>
</body>
</html>
