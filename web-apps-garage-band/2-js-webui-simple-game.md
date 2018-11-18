```
<html>
  <head>
    <style>
      body {
        font-family: arial;
        padding: 20px;
      }

      #header {
        font-size: xx-large;
      }

      #clickme {
        border: 1px solid black;
        background-color: blue;
        color: white;
        font-weight: bold;
        padding: 20px;
        display: inline-block;
        cursor: pointer;
      }

      #clicks {
        font-size: 100px;
        font-weight: bold;
        margin-top: 20px;
        margin-bottom: 20px;
      }

      .card {
        max-width: 200px;
        display: none;
      }
    </style>
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
  </head>

  <body>
    <div id=header>Welcome to our browser game</div> 

    <div id=clicks>0</div>

    <img id="egg" class="card" src="https://i.pinimg.com/originals/fc/b6/26/fcb626adad3e8e565f7ccb851d6a1b71.jpg"></img>
    <img id="hatchling" class="card" src="https://images-na.ssl-images-amazon.com/images/I/71FuuVDNbmL._SX425_.jpg"></img>

    <div class="wrapper">
      <div id="clickme">Click Me</div>
    </div>

    <script>
      $("#egg").show();

      var clickCounter = 0;

      // add click handler for button
      $("#clickme").click(
        function() {
          console.log( "HEHE THAT TICKLES!" );
          clickCounter += 1;          

          $("#clicks").html(clickCounter);

          // change picture after some clicks
          if (clickCounter > 10)
          {
            $(".card").hide();
            $("#hatchling").show();
          }
              
        }
      );

      
    </script>
  </body>
</html>
```
