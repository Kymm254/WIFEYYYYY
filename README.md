<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Valentine 💛</title>

  <style>
    body {
      margin: 0;
      height: 100vh;
      background: black;
      color: white;
      display: flex;
      justify-content: center;
      align-items: center;
      font-family: Arial, sans-serif;
      overflow: hidden;
    }

    .container {
      text-align: center;
    }

   h1 {
      font-size: 46px;
      font-weight: bold;
      margin-bottom: 20px;
    }

    img {
      width: 220px;
      margin: 20px 0;
    }

    button {
      font-size: 32px;
      font-weight: bold;
      padding: 20px 45px;
      margin: 15px;
      border-radius: 18px;
      border: 3px solid white;
      background: black;
      color: white;
      cursor: pointer;
    }

    #no {
      position: absolute;
    }
  </style>
</head>
<body>

  <div class="container">
<!-- Minion holding heart -->
    <img src="https://media.tenor.com/9yF7r3y6FhQAAAAi/minion-love.gif" alt="Minion
holding heart">

    <br>

    <button id="yes">❤️ YES ❤️</button>
    <button id="no">💔 NO 💔</button>
  </div>

  <script>
    const noBtn = document.getElementById("no");
    const yesBtn = document.getElementById("yes");

    noBtn.addEventListener("mouseover", () => {
      const x = Math.random() * (window.innerWidth - 220);
      const y = Math.random() * (window.innerHeight - 120);

      noBtn.style.left = x + "px";
      noBtn.style.top = y + "px";
    });

    yesBtn.addEventListener("click", () => {
      document.body.innerHTML = `
        <div style="text-align:center;color:white;">
          <h1 style="font-size:50px;">❤️ YAAAY ❤️</h1>
          <p style="font-size:28px;">
            You just made this Minion<br>
            and my heart very happy 🥰
          </p>
          <img src="https://media.tenor.com/fjZs9j2jv0sAAAAi/minion-hug.gif"
width="220">
        </div>
      `;
    });
  </script>

</body>
</html>

    <!-- Minion holding heart -->
