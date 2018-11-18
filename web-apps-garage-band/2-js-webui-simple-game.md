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
        font-size: 200px;
        font-weight: bold;
        margin-top: 20px;
        margin-bottom: 20px;
      }
    </style>
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
  </head>

  <body>
    <div id=header>Welcome to our browser game</div> 

    <div id=clicks>0</div>


    <div id="clickme">Click Me</div>

    <script>
      var clickCounter = 0;

      // add click handler for button
      $("#clickme").click(function() {
          console.log( "HEHE THAT TICKLES!" );
          clickCounter += 1;          

          $("#clicks").html(clickCounter);
      });

      
    </script>
  </body>
</html>
```
