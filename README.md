<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>PIX do Alemão</title>

  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: #000;
      color: white;
      text-align: center;
    }
    header {
      background: #111;
      padding: 30px;
    }
    header h1 {
      font-size: 2.5rem;
      margin: 0;
    }
    .container {
      padding: 40px 20px;
    }
    .pix-box {
      background: #222;
      border-radius: 10px;
      padding: 20px;
      margin: 20px auto;
      width: 90%;
      max-width: 400px;
    }
    .pix-box img {
      width: 200px;
      margin-bottom: 15px;
    }
    .btn-copy {
      background: #00cc66;
      color: white;
      padding: 12px 20px;
      border: none;
      border-radius: 7px;
      font-size: 1rem;
      cursor: pointer;
    }
    .btn-copy:hover {
      background: #00994d;
    }
    footer {
      margin-top: 50px;
      font-size: 0.8rem;
      color: #888;
    }
  </style>
</head>

<body>

  <header>
    <h1>PIX do Alemão</h1>
  </header>

  <div class="container">

    <div class="pix-box">
      <!-- Aqui pode colocar um QR Code se quiser -->
      <img src="https://via.placeholder.com/200" alt="QR Code PIX">
      <p><strong>Cópia e Cola PIX:</strong></p>
      <p id="pixCode">00020126360014BR.GOV.BCB.PIX0114+5511999999999205000053039865404100.00</p>
      <button class="btn-copy" onclick="copyPIX()">Copiar PIX</button>
    </div>

  </div>

  <footer>
    © 2026 PIX do Alemão — Todos os direitos reservados
  </footer>

  <script>
    function copyPIX() {
      const pixText = document.getElementById("pixCode").innerText;
      navigator.clipboard.writeText(pixText).then(() => {
        alert("PIX copiado com sucesso!");
      });
    }
  </script>

</body>
</html>
