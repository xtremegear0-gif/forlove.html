<!DOCTYPE html>
<html>
<head>
  <title>For My Wife ❤️</title>
</head>

<body>
  <h1>I Love You ❤️</h1>
  <p>You are my favorite person.</p>

  <button onclick="showMessage()">
    Click Me
  </button>

  <script>
    function showMessage() {
      alert("You mean everything to me ❤️");
    }
  </script>
</body>
</html>
# Romantic Animated Page ❤️

## Paste this inside your `love.html`

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>For My Wife ❤️</title>

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: Arial, sans-serif;
    }

    body {
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      background: linear-gradient(135deg, #ff758c, #ff7eb3);
      overflow: hidden;
      color: white;
      text-align: center;
    }

    .container {
      animation: fadeIn 2s ease;
      z-index: 2;
    }

    h1 {
      font-size: 55px;
      animation: glow 2s infinite alternate;
    }

    p {
      margin-top: 15px;
      font-size: 20px;
      opacity: 0.9;
      animation: slideUp 2s ease;
    }

    button {
      margin-top: 25px;
      padding: 15px 35px;
      border: none;
      border-radius: 50px;
      background: white;
      color: #ff4f81;
      font-size: 18px;
      cursor: pointer;
      transition: 0.3s;
    }

    button:hover {
      transform: scale(1.1);
      box-shadow: 0 0 20px white;
    }

    /* Floating hearts */
    .heart {
      position: absolute;
      width: 20px;
      height: 20px;
      background: red;
      transform: rotate(45deg);
      animation: float 8s linear infinite;
      opacity: 0.6;
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
      left: -10px;
      top: 0;
    }

    @keyframes float {
      0% {
        transform: translateY(100vh) rotate(45deg);
        opacity: 0;
      }

      100% {
        transform: translateY(-120vh) rotate(45deg);
        opacity: 1;
      }
    }

    @keyframes fadeIn {
      from {
        opacity: 0;
        transform: scale(0.8);
      }

      to {
        opacity: 1;
        transform: scale(1);
      }
    }

    @keyframes glow {
      from {
        text-shadow: 0 0 10px white;
      }

      to {
        text-shadow: 0 0 30px white;
      }
    }

    @keyframes slideUp {
      from {
        transform: translateY(50px);
        opacity: 0;
      }

      to {
        transform: translateY(0);
        opacity: 1;
      }
    }
  </style>
</head>

<body>

  <div class="container">
    <h1>For My Love ❤️</h1>
    <p>You make my world beautiful ✨</p>

    <button onclick="showLove()">
      Click Me ❤️
    </button>
  </div>

  <script>
    function showLove() {
      alert("I Love You Forever ❤️");
    }

    // Create floating hearts
    for (let i = 0; i < 25; i++) {
      let heart = document.createElement('div');
      heart.classList.add('heart');

      heart.style.left = Math.random() * 100 + 'vw';
      heart.style.animationDuration = (Math.random() * 5 + 5) + 's';
      heart.style.opacity = Math.random();

      document.body.appendChild(heart);
    }
  </script>

</body>
</html>
