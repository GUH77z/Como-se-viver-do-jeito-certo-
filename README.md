# Como-se-viver-do-jeito-certo-
Receba a inteligência 
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <title>Exemplo de Site</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #000;
      color: #fff;
      text-align: center;
      padding: 50px;
    }

    input[type="text"] {
      padding: 10px;
      width: 60%;
      font-size: 16px;
      margin-bottom: 10px;
      background-color: #111;
      color: #fff;
      border: 1px solid #444;
    }

    button {
      padding: 10px 20px;
      font-size: 16px;
      background-color: #ff9800;
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }

    #resposta {
      margin-top: 20px;
      font-size: 20px;
      font-style: italic;
    }

    body::before {
      content: "pdm's";
      position: fixed;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%) rotate(-30deg);
      font-size: 80px;
      color: rgba(255, 255, 255, 0.03);
      text-shadow: 0 0 15px rgba(255, 255, 255, 0.1);
      z-index: 0;
      pointer-events: none;
      user-select: none;
      white-space: nowrap;
    }
  </style>
</head>
<body>
  <h1>Digite algo:</h1>
  <input type="text" id="entrada" placeholder="Escreva aqui...">
  <br>
  <button onclick="mostrarResposta()">Enviar</button>
  <div id="resposta"></div>

  <script>
    function mostrarResposta() {
      const texto = document.getElementById('entrada').value;
      const resposta = document.getElementById('resposta');
      if (texto.trim() === "") {
        resposta.textContent = "Por favor, digite algo.";
      } else {
        resposta.textContent = `Você digitou: "${texto}"`;
      }
    }
  </script>
</body>
</html>
