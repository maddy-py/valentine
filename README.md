<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Be My Valentine ❤️</title>
  <style>
    body {
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      background: linear-gradient(135deg, #ff758c, #ff7eb3);
      font-family: Arial, sans-serif;
    }
 
    .box {
      background: white;
      padding: 40px;
      border-radius: 15px;
      text-align: center;
      box-shadow: 0 10px 30px rgba(0,0,0,0.2);
    }
 
    h1 {
      color: #ff4d6d;
    }
 
    button {
      padding: 12px 25px;
      font-size: 16px;
      margin: 15px;
      border: none;
      border-radius: 25px;
      cursor: pointer;
    }
 
    #yes {
      background: #ff4d6d;
      color: white;
    }
 
    #no {
      background: #ccc;
      position: absolute;
    }
  </style>
</head>
<body>
 
  <div class="box">
    <h1>Will you be my Valentine? 💖</h1>
    <button id="yes" onclick="yesClicked()">Yes ❤️</button>
    <button id="no">No 😏</button>
  </div>
 
  <script>
    const noBtn = document.getElementById("no");
 
    noBtn.addEventListener("mouseover", () => {
      const x = Math.random() * (window.innerWidth - 100);
      const y = Math.random() * (window.innerHeight - 50);
      noBtn.style.left = x + "px";
      noBtn.style.top = y + "px";
    });
 
    function yesClicked() {
      document.body.innerHTML = "<h1 style='color:white'>Yayyy! ❤️😍 I knew it!</h1>";
    }
  </script>
 
</body>
</html>
