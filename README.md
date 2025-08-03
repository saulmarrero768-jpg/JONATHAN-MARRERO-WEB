# JONATHAN-MARRERO-WEB
busco emplo como programador web
.presentacion {
    max-width: 700px;
    margin: 50px auto;
    background-color: #1e1e1e;
    color: #f5f5f5;
    padding: 30px;
    border-radius: 12px;
    box-shadow: 0 0 20px rgba(255, 0, 100, 0.3);
    font-family: 'Segoe UI', sans-serif;
  }
  
  .presentacion h1 {
    font-size: 36px;
    color: #ff0055;
    margin-bottom: 20px;
  }
  
  .presentacion p {
    font-size: 18px;
    line-height: 1.6;
  }
  
body {
    background: #f5f5f5;
    font-family: 'Arial', sans-serif;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    margin: 0;
  }
  
  .contact-card {
    background: white;
    padding: 30px 40px;
    border-radius: 20px;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
    text-align: center;
    max-width: 400px;
    width: 100%;
  }
  
  .contact-card h2 {
    margin-bottom: 20px;
    color: #333;
    font-size: 28px;
  }
  
  .contact-item {
    margin: 15px 0;
    font-size: 18px;
  }
  
  .contact-item i {
    margin-right: 10px;
    color: #555;
  }
  
  .contact-item a {
    color: #1a73e8;
    text-decoration: none;
    transition: color 0.3s;
  }
  
  .contact-item a:hover {
    color: #0d47a1;
  }
  img{
    height: 300px;
    width: 200;
    justify-content: center;
    align-items: center;

}

.btn-juego {
    display: inline-block;
    padding: 12px 24px;
    background: linear-gradient(135deg, #4f46e5, #3b82f6);
    color: white;
    text-decoration: none;
    font-weight: bold;
    border-radius: 12px;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.2);
    transition: all 0.3s ease;
    font-size: 16px;
    letter-spacing: 1px;
  }
  
  .btn-juego:hover {
    transform: scale(1.05);
    background: linear-gradient(135deg, #3b82f6, #60a5fa);
    box-shadow: 0 6px 16px rgba(0, 0, 0, 0.3);
  }

  .foto-presentacion {
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 20px auto;
  }
  
  .foto-presentacion img {
    width: 300px;
    height: 300px;
    object-fit: cover;
    border-radius: 50%;
    box-shadow: 0 8px 20px rgba(0, 0, 0, 0.3);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
    border: 4px solid #4f46e5;
  }
  
  .foto-presentacion img:hover {
    transform: scale(1.05);
    box-shadow: 0 16px 29px rgba(0, 0, 0, 0.4);
    border-color: #3b82f6;
  }
<!DOCTYPE html>
<html lang="en">
<head>
 
  <title>PAGINA</title>
  <link rel="stylesheet" href="estilos.css">
</head>


<body>
  <section class="presentacion">
    <h1>Hola, soy Jonathan</h1>
    <p>Tengo 18 años, soy cubano y me apasiona la programación.</p>
    <p>Desde que descubrí el código, puedo pasar horas y días programando sin darme cuenta.</p>
    <p>Tengo experiencia en <strong>HTML</strong>, <strong>CSS</strong> y <strong>JavaScript</strong>.</p>
    <p> En esta página comparto un poco de mí y de mis proyectos. Estoy buscando empleo como programador freelance o en equipo. LES DEJE DOS MINI JUEGOS A LA DERECHA</p>
  </section>
<br>

  <div
 class="foto-presentacion">  <img src="IMG_7660.JPG" alt="Foto de Jonathan">



  </div>

  
  
  
  
  
  
  
  
  
  
  
  <div class="contact-card">
    <h2>Contáctame</h2>
    <div class="contact-item">
      <i class="fab fa-whatsapp"></i>
      <a href="https://wa.me/5358736471" target="_blank">+53 58736471</a>
    </div>
    <div class="contact-item">
      <i class="fab fa-instagram"></i>
      <a href="https://instagram.com/jonathanmarreror" target="_blank">@jonathanmarreror</a>
    </div>
  </div>
  
  
  
  <div>
    <a href="otro.html" class="btn-juego" target="_blank">Ir al Juego 1</a>
    <a href="juego.html" class="btn-juego" target="_blank">Ir al Juego 2</a>
  </div>
  




</body>
</html>
<nav>
    <ul>
 <li><a href="#CONTACTO">CONTACTO</a></li>
 </ul>
 </nav>
 
 <a href="https://wa.me/58736471" 
 target=blank"> ESCRIBEME AL WHATSAPP</a>
 
 
 <H5>ENCUENTRA EL BOTON CORRECTO</H5>
 <button class="boton"
   onclick="verificar(this)">Boton 1<button>
     <button class="boton"
     onclick="verificar(this)">Boton 2<button>
       <button class="boton"
       onclick="verificar(this)">Boton 3<button>
 
         <div class="mensaje" id="resultado"></div>
 
         <script>
           const correcto =
           Math.floor(Math.random() * 3);
 
           function verificar(boton) {
             const botones = 
             document.querySelectorAll(".boton");
             
             const index = 
             Array.from(botones).indexOf(boton);
             const resultado =
             document.getElementById("resultado");
           if (index === correcto) { 
             resultado.textContent = "CORRECTO!";
             resultado.style.color = "lime"; 
           } else { 
             resultado.textContent = "INTENTA OTRA VEZ.";
             resultado.style.color = "red";
             }
           }
             
    </script>
 <br>
 
 
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Mini Juego - Adivina el Número</title>
  <style>
    body {
      background-color: #111;
      color: #fff;
      font-family: 'Segoe UI', sans-serif;
      text-align: center;
      padding: 50px;
    }

    h1 {
      color: #ff0077;
    }

    input, button {
      padding: 10px;
      margin: 10px;
      font-size: 16px;
      border-radius: 8px;
      border: none;
    }

    #mensaje {
      margin-top: 20px;
      font-size: 18px;
      color: #00ff99;
    }

    .contenedor {
      background-color: #222;
      padding: 30px;
      border-radius: 12px;
      box-shadow: 0 0 20px #ff007766;
      max-width: 400px;
      margin: auto;
    }
  </style>
</head>
<body>
  <div class="contenedor">
    <h1>🎯 Adivina el Número</h1>
    <p>Estoy pensando en un número del 1 al 10. ¿Puedes adivinar cuál es?</p>
    <input type="number" id="entrada" min="1" max="10">
    <button onclick="adivinar()">Adivinar</button>
    <p id="mensaje"></p>
  </div>

  <script>
    let numeroSecreto = Math.floor(Math.random() * 10) + 1;

    function adivinar() {
      let intento = parseInt(document.get
