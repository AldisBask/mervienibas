<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Attaluma mervienibas</title>
</head>

<head>
  <style>
    h1 {
      font-size: 30px;

    }

    body {
      background: url(https://images.pexels.com/photos/577696/pexels-photo-577696.jpeg);
      background-position:center;
      background-size: cover;
      color: darkgray;
        
          }
          
     input{
         padding: 10px;
         margin: 10px;
         text-align: center;
         font-size: 20px;
         
         }
              
  </style>
  <script>
  
 function aprekinatjudzes()
 {
     let km = $("#kilometri").val();
     
     $("#judzes").val( (km*0.62137119).toFixed(3) );
 }
   
 function aprekinatkilometrus()
 {
     let judzes = $("#judzes").val();
     
     $("#kilometri").val( (judzes/0.62137119).toFixed(3) );
 }
 
  </script>
</head>

<body>
  <center>
    <h1>Attaluma mērvienību pārveidotājs</h1>
    
    Kilometri:<br>
    <input type="text" id="kilometri" onkeyup="aprekinatjudzes()">
    <br>
    
    Jūdzes:<br>
    <input type="text" id= "judzes"  onkeyup="aprekinatkilometrus()">
    <br>
        
    
  </center>

</body>

</html>
