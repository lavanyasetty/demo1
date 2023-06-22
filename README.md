<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-9ndCyUaIbzAi2FUVXJi0CjmCapSmO7SnpJef0486qhLnuZ2cdeRhO02iuK6FUUVM" crossorigin="anonymous">
    <link rel="stylesheet" href="C:\Users\LAVANYA\Documents\bharatIntern projects\temperature converter\style.css">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    
  <div class="container">
     <h3>Temperature converter from Celsius to fahrenheit</h3>   
     <p>Type a value in the Fahrenheit field to convert the value to Celsius:</p>
     
        <label>Fahrenheit</label>
        <input id="inputFahrenheit" class="form-control" type="number" placeholder="Fahrenheit" oninput="temperatureConverter(this.value)" onchange="temperatureConverter(this.value)">
     
   <p>Celcius: <span id="outputCelcius"></span></p>
   
</div>

   <script>
   function temperatureConverter(valNum) {
     valNum = parseFloat(valNum);
     document.getElementById("outputCelcius").innerHTML=(valNum-32)/1.8;
   }
</script>
</body>
</html>
