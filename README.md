# wkwk
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Puisi Romantis</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      background: linear-gradient(to right, #ff9a9e, #fad0c4);
      font-family: 'Segoe UI', sans-serif;
      color: white;
      overflow: hidden;
    }

    .container {
      text-align: center;
      padding: 20px;
      position: relative;
      z-index: 10;
    }

    img {
      width: 200px;
      height: 200px;
      object-fit: cover;
      border-radius: 50%;
      border: 4px solid white;
      margin-bottom: 20px;
      box-shadow: 0 5px 15px rgba(0,0,0,0.3);
    }

    h1 {
      font-size: 1.8em;
      margin-bottom: 10px;
    }

    p {
      font-size: 1.2em;
      line-height: 1.6;
      padding: 0 15px;
    }

    .heart {
      position: fixed;
      width: 20px;
      height: 20px;
      background: red;
      transform: rotate(45deg);
      animation: float 5s linear infinite;
      opacity: 0.7;
    }

    .heart::before,
    .heart::after {
      content: '';
      position: absolute;
      width: 20px;
      height: 20px;
      background: red;
      border-radius: 50%;
    }

    .heart::before {
      top: -10px;
      left: 0;
    }

    .heart::after {
      top: 0;
      left: -10px;
    }

    @keyframes float {
      0% {
        transform: translateY(0) rotate(45deg);
        opacity: 1;
      }
      100% {
        transform: translateY(-100vh) rotate(45deg);
        opacity: 0;
      }
    }
  </style>
</head>
<body>
  <div class="container">
    <img src="https://i.ibb.co/yFsXMnP/love-photo.jpg" alt="Foto Romantis" />
    <h1>Untukmu, yang Selalu di Hatiku</h1>
    <p>
      Dalam diam, aku menyebut namamu<br>
      Dalam hujan, aku rindukan teduhmu<br>
      Di setiap hembus napasku, ada namamu<br>
      Cintaku padamu... tak pernah surut, tak pernah usai<br><br>
      Kau adalah puisiku yang tak selesai
    </p>
  </div>

  <script>
    // Fungsi animasi love
    function createHeart() {
      const heart = document.createElement('div');
      heart.classList.add('heart');
      heart.style.left = Math.random() * 100 + 'vw';
      heart.style.animationDuration = 3 + Math.random() * 2 + 's';
      document.body.appendChild(heart);

      setTimeout(() => {
        heart.remove();
      }, 5000);
    }

    setInterval(createHeart, 300);
  </script>
</body>
</html>
<img src="https://ibb.co.com/50s0RY2 "alt="Foto Romantis" />
