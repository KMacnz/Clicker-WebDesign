<!DOCTYPE html>
<html id="index">
  <head>
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <meta name="author" content="Keanna">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
    <link href='https://fonts.googleapis.com/css?family=Alfa+Slab+One' rel='stylesheet'>
    <link href='https://fonts.googleapis.com/css?family=Bree+Serif' rel='stylesheet'>
    <link href='https://fonts.googleapis.com/css?family=Muli' rel='stylesheet'>
    <link href='https://fonts.googleapis.com/css?family=Varela+Round' rel='stylesheet'>
    <link href='https://fonts.googleapis.com/css?family=Francois+One' rel='stylesheet'>
    <link href='https://fonts.googleapis.com/css?family=Kanit' rel='stylesheet'>
    <link href='https://fonts.googleapis.com/css?family=Hammersmith+One' rel='stylesheet'>
    <link rel="stylesheet" href="clickerstyles.css">
  </head>
  <body style="background-color:#80C2AF">
    <div class='whiteContainer'>
      <div class="container">
        <a href="clicker.html">Reset</a>
        </div>
        <h1 align="center">Cookie Clicker</h1>
       <h2 align="center">Try To Win!!!</h2>
       <section>
       <script>
       var total = 0;
       var multiplyier = 1;
       function clicker(){
         total = total + (1 * multiplyier);
         document.getElementById("counter").innerHTML = total;
       }
       </script>
       <button onclick="clicker()">Click Me</button>
       <button onclick="bonus()">Go Faster</button>
       <p id = "counter">0</p>
     </section>
  </body>
</html>
<Version 1: Web Design and CSS Code Sorted
Version 2: Button and Values of Clicks>
