<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Vamos tomar açaí amanhã?</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      background-color: #f0f8ff;
      padding: 50px;
    }

    h1 {
      color: #2c3e50;
    }

    .button {
      background-color: #4CAF50;
      color: white;
      padding: 15px 32px;
      font-size: 20px;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      margin: 20px;
      transition: background-color 0.3s;
    }

    .button:hover {
      background-color: #45a049;
    }

    .button-errado {
      background-color: #e74c3c;
    }

    .message {
      margin-top: 30px;
      font-size: 18px;
      color: #2980b9;
    }
  </style>
</head>
<body>

  <h1>Vamos tomar açaí amanhã?</h1>

  <button class="button" onclick="resposta('sim')">Sim</button>
  <button class="button button-errado" onclick="resposta('nao')">Não</button>

  <div id="mensagem" class="message"></div>

  <script>
    function resposta(opcao) {
      let mensagem = document.getElementById('mensagem');

      if (opcao === 'sim') {
        mensagem.innerHTML = "Marcado!";
        mensagem.style.color = "green";
      } else if (opcao === 'nao') {
        mensagem.innerHTML = "Resposta errada, tente novamente.";
        mensagem.style.color = "red";
      }
    }
  </script>

</body>
</html>
