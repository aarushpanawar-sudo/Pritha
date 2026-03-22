# Pritha
<!DOCTYPE html><html>
<head>
  <title>I'm Sorry ❤️</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: 'Segoe UI', sans-serif;
      background: linear-gradient(to bottom, #ffd6e0, #fff);
      text-align: center;
      overflow: hidden;
    }h1 {
  color: #ff4d6d;
  margin-top: 50px;
  font-size: 40px;
  animation: fadeIn 2s ease-in-out;
}

p {
  font-size: 18px;
  color: #444;
  margin: 20px;
  animation: fadeIn 3s ease-in-out;
}

button {
  background: #ff4d6d;
  color: white;
  border: none;
  padding: 12px 25px;
  border-radius: 25px;
  font-size: 16px;
  cursor: pointer;
  transition: 0.3s;
}

button:hover {
  background: #e63950;
  transform: scale(1.1);
}

.message {
  display: none;
  background: white;
  margin: 20px auto;
  padding: 20px;
  width: 80%;
  max-width: 400px;
  border-radius: 20px;
  box-shadow: 0 10px 30px rgba(0,0,0,0.1);
  animation: pop 0.6s ease;
}

.heart {
  position: absolute;
  color: red;
  animation: float 6s linear infinite;
}

@keyframes float {
  0% { transform: translateY(100vh); opacity: 1; }
  100% { transform: translateY(-10vh); opacity: 0; }
}

@keyframes fadeIn {
  from { opacity: 0; }
  to { opacity: 1; }
}

@keyframes pop {
  from { transform: scale(0.5); opacity: 0; }
  to { transform: scale(1); opacity: 1; }
}

  </style>
</head>
<body>  <h1>I'm Really Sorry 💔</h1>
  <p>I never meant to hurt you... please hear me out 🥺</p><button onclick="showMessage()">Click Me 💌</button>

  <div class="message" id="msg">
    <h2>Dear Love ❤️</h2>
    <p>
      I'm truly sorry for what I did.
      <br><br>
      You mean the world to me, and I hate seeing you upset because of me.
      <br><br>
      Please forgive me... I promise to do better 💖
    </p>
  </div>  <script>
    function showMessage() {
      document.getElementById("msg").style.display = "block";
    }

    // Floating hearts
    setInterval(() => {
      const heart = document.createElement("div");
      heart.classList.add("heart");
      heart.innerHTML = "❤️";
      heart.style.left = Math.random() * 100 + "vw";
      heart.style.fontSize = Math.random() * 20 + 20 + "px";
      document.body.appendChild(heart);

      setTimeout(() => {
        heart.remove();
      }, 6000);
    }, 300);
  </script></body>
</html>
