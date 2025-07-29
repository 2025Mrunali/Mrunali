<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Login Page</title>
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
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
    }

    .login-container {
      background-color: #fff;
      padding: 20px;
      border-radius: 8px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
      width: 300px;
    }

    form h2 {
      text-align: center;
      margin-bottom: 20px;
    }

    .input-group {
      margin-bottom: 15px;
    }

    .input-group label {
      display: block;
      font-size: 14px;
      margin-bottom: 5px;
    }

    .input-group input {
      width: 100%;
      padding: 8px;
      border: 1px solid #ddd;
      border-radius: 4px;
    }

    button {
      width: 100%;
      padding: 10px;
      background-color: #007bff;
      color: #fff;
      border: none;
      border-radius: 4px;
      cursor: pointer;
    }

    button:hover {
      background-color: #0056b3;
    }

    .error {
      color: red;
      font-size: 12px;
      margin-bottom: 15px;
    }
  </style>
</head>
<body>

  <div class="login-container">
    <form id="loginForm">
      <h2>Login</h2>
      
      <div class="input-group">
        <label for="username">Username</label>
        <input type="text" id="username" name="username" required>
      </div>
      
      <div class="input-group">
        <label for="password">Password</label>
        <input type="password" id="password" name="password" required>
      </div>

      <div class="error" id="error-message"></div>
      
      <button type="submit">Login</button>
    </form>
  </div>

  <script>
    document.getElementById('loginForm').addEventListener('submit', function (event) {
      event.preventDefault(); // Prevent form submission
      
      const username = document.getElementById('username').value;
      const password = document.getElementById('password').value;
      const errorMessage = document.getElementById('error-message');

      // Clear any previous error messages
      errorMessage.textContent = '';

      // Basic validation
      if (username === '' || password === '') {
        errorMessage.textContent = 'Please fill out both fields.';
      } else if (username !== 'admin' || password !== 'password123') {
        errorMessage.textContent = 'Invalid username or password.';
      } else {
        // Simulate successful login (you can redirect here)
        alert('Login Successful');
        // Redirect (optional)
        // window.location.href = 'home.html';
      }
    });
  </script>

</body>
</html>
