
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Simple Webpage</title>
  <style>
    /* Basic Reset */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: Arial, sans-serif;
      background-color: #f4f7fc;
      padding: 20px;
      display: flex;
      flex-direction: column;
      align-items: center;
    }

    header {
      width: 100%;
      background-color: #4CAF50;
      color: white;
      padding: 20px;
      text-align: center;
    }

    .content {
      width: 80%;
      max-width: 800px;
      margin: 20px 0;
      background-color: #fff;
      padding: 20px;
      border-radius: 8px;
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    }

    h1 {
      font-size: 32px;
      margin-bottom: 10px;
    }

    p {
      font-size: 18px;
      line-height: 1.6;
      margin-bottom: 20px;
    }

    .button-container {
      text-align: center;
    }

    button {
      padding: 10px 20px;
      background-color: #007bff;
      color: white;
      border: none;
      border-radius: 5px;
      font-size: 16px;
      cursor: pointer;
    }

    button:hover {
      background-color: #0056b3;
    }

    img {
      width: 100%;
      max-width: 100%;
      border-radius: 8px;
      margin-top: 20px;
    }
  </style>
</head>
<body>

  <header>
    <h1>Welcome to My Simple Webpage</h1>
    <p>This is an example of a webpage with HTML, CSS, and JS all in one file.</p>
  </header>

  <div class="content">
    <h2>About This Page</h2>
    <p>
      This is a simple webpage designed to showcase a webpage structure with HTML, CSS, and JavaScript integrated into a single file.
      The page includes a header, a main content section with an image, and a button that changes the background color of the page.
    </p>

    <img src="https://via.placeholder.com/800x400" alt="Placeholder Image">

    <div class="button-container">
      <button onclick="changeBackgroundColor()">Change Background Color</button>
    </div>
  </div>

  <script>
    // JavaScript function to change background color
    function changeBackgroundColor() {
      // Generate a random color
      const colors = ['#ff7f7f', '#7fffd4', '#ffd700', '#f0e68c', '#add8e6', '#98fb98'];
      const randomColor = colors[Math.floor(Math.random() * colors.length)];
      document.body.style.backgroundColor = randomColor;
    }
  </script>

</body>
</html>
