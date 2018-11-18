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

    <script>
      $("#header")
        .html("Welcome, friend!");

      $(".paragraph").css("font-weight", "bold");
    </script>
  </body>
</html>
```
