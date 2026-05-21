# osbaldoguerrero.github.io
<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8" />
  <title>Sound Button</title>

  <style>
    body{
      margin:0;
      display:flex;
      justify-content:center;
      align-items:center;
      height:100vh;
      background:transparent;
    }

    #soundBtn{
      width:220px;
      cursor:pointer;
      transition:transform 0.1s;
    }

    #soundBtn:active{
      transform:scale(0.95);
    }
  </style>
</head>

<body>

  <img
    id="soundBtn"
    src="https://res.cloudinary.com/dkyjcwocf/image/upload/v1779325178/Peinados_13_cmap3b.png"
  />

  <audio id="audio">
    <source src="https://res.cloudinary.com/dkyjcwocf/video/upload/q_auto/f_auto/v1779325295/Toten-t%C3%A1ns_Liszt_El_final_El_c_Professor_MiniMax_02_HD_019e32a3-ea30-7340-8681-1aee8c42ec5b_mfxyxp.mp3" type="audio/mpeg">
  </audio>

  <script>
    const btn = document.getElementById("soundBtn");
    const audio = document.getElementById("audio");

    btn.addEventListener("click", () => {
      audio.currentTime = 0;
      audio.play();
    });
  </script>

</body>
</html>
