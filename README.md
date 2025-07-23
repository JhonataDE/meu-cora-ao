<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Meu coração é seu</title>
  <style>
    body {
      background: #fff0f5;
      font-family: Arial, sans-serif;
      text-align: center;
      padding: 50px;
    }

    h1 {
      color: #e91e63;
    }

    #heart {
      font-size: 100px;
      color: red;
      display: none;
      animation: beat 1s infinite;
    }

    @keyframes beat {
      0%, 100% { transform: scale(1); }
      50% { transform: scale(1.2); }
    }

    #message {
      margin-top: 20px;
      font-size: 24px;
      color: #e91e63;
      display: none;
    }

    button {
      padding: 15px 25px;
      font-size: 20px;
      background-color: #e91e63;
      color: white;
      border: none;
      border-radius: 10px;
      cursor: pointer;
    }

    button:hover {
      background-color: #d81b60;
    }
  </style>
</head>
<body>

  <h1>💌 Clique no botão abaixo 💌</h1>
  <button onclick="mostrarAmor()">Clique aqui</button>

  <div id="heart">❤️</div>
  <div id="message">Você tem meu coração!</div>

  <script>
    function mostrarAmor() {
      document.getElementById('heart').style.display = 'block';
      document.getElementById('message').style.display = 'block';
    }
  </script>

</body>
</html>
