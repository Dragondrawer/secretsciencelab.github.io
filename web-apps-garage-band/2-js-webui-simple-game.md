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

      .paragraph {
        font-style: italic;
        margin: 20px;
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
    </style>
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
  </head>

  <body>
    <div id=header>Welcome</div> 

    <div class=paragraph>
      Some text
      Some text
      Some text
      Some text
    </div> 
    <div class=paragraph>
      Some text 2
      Some text 2
      Some text 2
      Some text 2
    </div> 

    <div id="clickme">Click Me</div>

    <script>
      function runThisWhenClicked() {
        alert( "HEHE THAT TICKLES!" );
      }

      // add click handler for button
      $("#clickme").click(runThisWhenClicked);

      
    </script>
  </body>
</html>
```
