# Name-site
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Welcome Page</title>
  <style>
    body {
      font-family: "Poppins", sans-serif;
      background: linear-gradient(135deg, #d7e1ec, #f0f3f8);
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
      color: #222;
    }

    .card {
      background: #fff;
      padding: 35px 40px;
      border-radius: 16px;
      box-shadow: 0 8px 20px rgba(0,0,0,0.1);
      text-align: center;
      width: 90%;
      max-width: 350px;
    }

    h1 {
      font-size: 24px;
      color: #333;
      margin-bottom: 10px;
    }

    p {
      color: #555;
      margin-bottom: 20px;
    }

    input {
      padding: 10px;
      width: 85%;
      border: 2px solid #ccc;
      border-radius: 8px;
      font-size: 16px;
      outline: none;
      transition: border 0.3s;
    }

    input:focus {
      border-color: #6c63ff;
      box-shadow: 0 0 5px rgba(108, 99, 255, 0.3);
    }

    button {
      margin-top: 15px;
      padding: 10px 25px;
      background-color: #6c63ff;
      color: white;
      border: none;
      border-radius: 8px;
      font-size: 16px;
      cursor: pointer;
      transition: background 0.3s;
    }

    button:hover {
      background-color: #5a52e0;
    }

    .message {
      margin-top: 25px;
      font-size: 18px;
      color: #222;
    }
  </style>
</head>
<body>

  <div class="card">
    <h1>What is your name?</h1>
    <p>Type your name below 👇</p>
    <input type="text" id="nameInput" placeholder="Enter your name" />
    <br>
    <button onclick="showMessage()">Submit</button>

    <div class="message" id="message"></div>
  </div>

  <script>
    function showMessage() {
      const name = document.getElementById("nameInput").value.trim();
      const messageBox = document.getElementById("message");

      if (name === "") {
        messageBox.textContent = "Please enter your name!";
        return;
      }

      // 💬 You can change this sentence to whatever you like below 👇
      const customSentence = `Hey ${name} fuck you ! 🌟`;

      messageBox.textContent = customSentence;
    }
  </script>

</body>
</html>
