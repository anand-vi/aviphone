<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mobile features display website design</title>
    <link rel="stylesheet" href="realphone.css">
  </head>
  <body>
    <div class="main">
      <nav>
        <div class="logo">
          <img src="./images/logo.png">
        </div>
        <div class="nav-links">
          <ul>
            <li> <a href="#"> Home</a></li>
            <li> <a href="#"> Phone</a></li>
            <li> <a href="#"> Accessories</a></li>
            <li> <a href="#"> Cart</a></li>
          </ul>
        </div>
      </nav>
      <div class="information">
        <div class="overlay"></div>
        <img src="./images/mobile.png" class="mobile">
        <div id="circle">
          <div class="feature one">
            <img src="./images/camera.png">
            <div>
              <h1> Camera</h1>
              <P>12MP, Wide Angle Lens</P>
            </div>  
          </div>
          <div class="feature two"> 
            <img src="./images/processor.png">
            <div>
              <h1>Processor</h1>
              <P>Snapdragon Octa-core 11nm </P>
            </div>
          </div>
          <div class="feature three">
            <img src="./images/display.png">
            <div>
              <h1> Display</h1>
              <P>6.5" Mini-Drop Fullscreen </P>
            </div>
          </div>
          <div class="feature four"> 
            <img src="./images/battery.png">
            <div>
              <h1> Battery Life</h1>
              <P>5000mAh, 720Hrs  Standby </P>
            </div>
          </div>
        </div>
      </div>
      <div class="controls">
        <img src="./images/arrow.png" id="upBtn">
        <h3>Features</h3>
        <img src="./images/arrow.png" id="downBtn">
      </div>
    </div>
    <script>
      var circle = document.getElementById("circle");
      var upBtn = document.getElementById("upBtn");
      var downBtn = document.getElementById("downBtn");
      var  rotateValue = circle.style.transform;
      var rotateSum;
      upBtn.onclick = function()
      {
        rotateSum = rotateValue + "rotate(-90deg)";
        circle.style.transform = rotateSum;
        rotateValue = rotateSum;
      }
      downBtn.onclick = function()
      {
        rotateSum = rotateValue + "rotate(90deg)";
        circle.style.transform = rotateSum;
        rotateValue = rotateSum;
      }
    </script>
  </body>
</html>
