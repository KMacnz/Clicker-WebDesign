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
      <!-- My Java Script Code is between the script section -->
       <script>
         <!-- tells you that you are making a new variable and you saving items in it -->
       var total = 0;
       var multipler = 1;
        <!-- fuction tell the clicker what to do, this funtion is telling the clicker that each click is one point plus a bonus in the multiplyer-->
       function clicker() {
           total = total + multipler;
           document.getElementById("counter").innerHTML = total;
           <!-- if the value of the counter is greater than 9 inable the button -->
           if(total > 9) {
              document.getElementById("bonusButton").disabled = false;
           }
       }
       <!-- if the counter has 10 or more it will only minus ten points not all of your points -->
       function bonus() {
           multipler = multipler + 1;
           total = total - 10;

           document.getElementById("counter").innerHTML = total;
           <!-- if the counter has less than 10 the go faster button will be disabled -->
           if(total < 10) {
               document.getElementById("bonusButton").disabled=true;
           }
       }
   </script>
   <!-- these are the buttons that you click for the game -->
   <button id="clickButton" onclick="clicker()"><img width="250" src="https://eleventhstack.files.wordpress.com/2013/06/chocolate_chip_cookies.jpg"></button>
   <!-- these are the buttons that you click for the game this one is disable unless you have more than ten points-->
   <button id="bonusButton" onclick="bonus()" disabled=true>Go faster</button>

   <p id="counter"></p>

     </section>
  </body>
</html>
<!-- These are my versions of the Website
Version 1: Web Design and CSS Code Sorted
Version 2: Button and Values of Clicks
Version 3: Another Button Added and More Values
Version 4: Add Images and Comments
-->
