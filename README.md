# Brecho-oonlinet
<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Brechó Oonlinet</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f9f9f9;
      margin: 0;
      padding: 0;
      color: #333;
    }
    header {
      background-color: #000;
      color: #fff;
      text-align: center;
      padding: 20px 10px;
    }
    nav {
      text-align: center;
      padding: 10px;
      background-color: #111;
    }
    nav a {
      color: white;
      margin: 0 10px;
      text-decoration: none;
    }
    .slider {
      width: 100%;
      max-height: 300px;
      overflow: hidden;
      position: relative;
    }
    .slides {
      display: flex;
      width: 300%;
      animation: slide 12s infinite;
    }
    .slides img {
      width: 100%;
      height: auto;
      object-fit: cover;
    }
    @keyframes slide {
      0% { transform: translateX(0%); }
      33% { transform: translateX(-100%); }
      66% { transform: translateX(-200%); }
      100% { transform: translateX(0%); }
    }
    .catalogo {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
      padding: 20px;
    }
    .produto {
      background-color: #fff;
      border-radius: 8px;
      padding: 15px;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
      text-align: center;
    }
    .produto img {
      max-width: 100%;
      height: auto;
      border-radius: 6px;
    }
    footer {
      background-color: #000;
      color: #fff;
      text-align: center;
      padding: 15px;
      margin-top: 30px;
    }
    .botao-whatsapp, .botao-pix {
      color: white;
      padding: 10px 15px;
      display: inline-block;
      margin-top: 10px;
      border-radius: 5px;
      text-decoration: none;
      cursor: pointer;
    }
    .botao-whatsapp {
      background-color: #25D366;
    }
    .botao-pix {
      background-color: #6d28d9;
    }
  </style>
</head>
<body>
  <header>
    <h1>Brechó Oonlinet</h1>
    <p>Os melhores Nike Air Max TN por apenas R$150!</p>
  </header>

  <nav>
    <a href="#catalogo">Catálogo</a>
    <a href="#contato">Contato</a>
    <a href="https://instagram.com/brecho_oonlinet" target="_blank">Instagram</a>
  </nav>

  <div class="slider">
    <div class="slides">
      <img src="imagens/IMG-20250624-WA0036.jpg" alt="Air Max TN Branco" />
      <img src="imagens/IMG-20250624-WA0035.jpg" alt="Air Max TN Preto" />
      <img src="imagens/IMG-20250624-WA0037.jpg" alt="Air Max TN Deadpool" />
    </div>
  </div>

  <section id="catalogo" class="catalogo">
    <div class="produto">
      <img src="imagens/IMG-20250624-WA0036.jpg" alt="Air Max TN Branco" />
      <h3>Nike Air Max TN Branco</h3>
      <p>R$ 150,00</p>
      <a class="botao-whatsapp" href="https://wa.me/5551991215716?text=Quero+comprar+o+Nike+Air+Max+TN+Branco">Comprar</a><br />
      <span class="botao-pix" onclick="copiarPix()">Copiar Pix</span>
    </div>
    <div class="produto">
      <img src="imagens/IMG-20250624-WA0035.jpg" alt="Air Max TN Preto" />
      <h3>Nike Air Max TN Preto</h3>
      <p>R$ 150,00</p>
      <a class="botao-whatsapp" href="https://wa.me/5551991215716?text=Quero+comprar+o+Nike+Air+Max+TN+Preto">Comprar</a><br />
      <span class="botao-pix" onclick="copiarPix()">Copiar Pix</span>
    </div>
    <div class="produto">
      <img src="imagens/IMG-20250624-WA0037.jpg" alt="Air Max TN Deadpool" />
      <h3>Nike Air Max TN Deadpool</h3>
      <p>R$ 150,00</p>
      <a class="botao-whatsapp" href="https://wa.me/5551991215716?text=Quero+comprar+o+Nike+Air+Max+TN+Deadpool">Comprar</a><br />
      <span class="botao-pix" onclick="copiarPix()">Copiar Pix</span>
    </div>
    <div class="produto">
      <img src="https://via.placeholder.com/250x200?text=Air+Max+TN+Venom" alt="Air Max TN Venom" />
      <h3>Nike Air Max TN Venom</h3>
      <p>R$ 150,00</p>
      <a class="botao-whatsapp" href="https://wa.me/5551991215716?text=Quero+comprar+o+Nike+Air+Max+TN+Venom">Comprar</a><br />
      <span class="botao-pix" onclick="copiarPix()">Copiar Pix</span>
    </div>
  </section>

  <footer id="contato">
    <p>WhatsApp: <a href="https://wa.me/5551991215716" style="color: #25D366">(51) 99121-5716</a></p>
    <p>Email: <a href="mailto:eliezetbombieri@gmail.com" style="color: #25D366">eliezetbombieri@gmail.com</a></p>
    <p>Siga no Instagram: <a href="https://instagram.com/brecho_oonlinet" target="_blank" style="color: #25D366">@brecho_oonlinet</a></p>
  </footer>

  <script>
    function copiarPix() {
      const chavePix = "048.363.760-25";
      navigator.clipboard.writeText(chavePix).then(() => {
        alert("Chave Pix copiada: " + chavePix);
      });
    }
  </script>
</body>
</html>
