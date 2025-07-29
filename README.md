<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>One Page CSS Example</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f2f2f2;
      margin: 0;
      padding: 20px;
    }
    h1 {
      color: #333;
      text-align: center;
    }
    p {
      color: #555;
      line-height: 1.6;
    }
    .container {
      background-color: white;
      padding: 20px;
      border-radius: 10px;
      max-width: 600px;
      margin: auto;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
    }
    .button {
      display: inline-block;
      padding: 10px 15px;
      background-color: #007BFF;
      color: white;
      text-decoration: none;
      border-radius: 5px;
    }
    .button:hover {
      background-color: #0056b3;
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>Welcome to My Page</h1>
    <p>This is a simple demonstration of how HTML and CSS can be combined in a single document. The CSS styles are defined in the `<style>` section of the head and applied to elements in the body.</p>
    <a href="#" class="button">Click Me</a>
  </div>
</body>
</html>
