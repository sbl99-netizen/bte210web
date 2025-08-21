# bte210web

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Date & Time Display</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      margin-top: 100px;
      background-color: #f9f9f9;
    }
    button {
      padding: 10px 20px;
      font-size: 16px;
      border: none;
      border-radius: 8px;
      background-color: #4CAF50;
      color: white;
      cursor: pointer;
    }
    button:hover {
      background-color: #45a049;
    }
    #output {
      margin-top: 20px;
      font-size: 18px;
      color: #333;
    }
  </style>
</head>
<body>
  <h1>Show Today's Date & Time</h1>
  <button onclick="showDateTime()">Click Me</button>
  <div id="output"></div>

  <script>
    function showDateTime() {
      const now = new Date();
      const formatted = now.toLocaleString(); // Formats to local date & time
      document.getElementById("output").innerText = "Current Date & Time: " + formatted;
    }
  </script>
</body>
</html>
