# Temperature-Converter
2nd task of Web Development internship given by Bharat Intern.

<!DOCTYPE html>
<html>
<head>
  <title>Temperature Converter</title>
  <style>
    header{
  background-color: rgb(177, 172, 45);
    }
    body {
      font-family: Arial, sans-serif;
      padding: 30px;
      background-color: rgb(207, 205, 150);
    }
    
    .container {
      margin: 150px auto;
      width: 300px;

    }
    
    h1 {
      text-align: center;
    }
    
    label {
      display: block;
      margin-bottom: 5px;
    }
    
    input {
      width: 100%;
      padding: 5px;
      margin-bottom: 10px;
    }
    
    button {
      width: 100%;
    padding: 10px;
    background-color: #210d71;
    color: white;
    cursor: pointer;
    border: white;
    margin-bottom: 10px;
    }
    
    .result {
      font-weight: bold;
      text-align: center;
      margin-top: 20px;
    }
    footer{
      align-content: center;
    }
    footer{
      margin-top: -20px;
      text-align: center;
    }
  
    body hr{
      border: 0;
    background-color: rgb(110, 110, 155);
    height: 2px;
    margin: 60px 84px;
    }
  </style>
</head>
<body>
  <header>
    <h1>Temperature Converter</h1>
    
  </header>
  <div class="container">
    
    <label>Temperature (Celsius)</label>
    <input type="number" id="celsiusInput">
    
    <button onclick="convertToCelsius()">Convert to Fahrenheit</button>
    <button onclick="convertToFahrenheit()">Convert to Celsius</button>
    
    <div class="result" id="result">
      <h3>Result!!</h3>
    </div>
  </div>

  <script>
    function convertToCelsius() {
      var celsius = parseFloat(document.getElementById("celsiusInput").value);
      var fahrenheit = (celsius * 9/5) + 32;
      document.getElementById("result").innerHTML = celsius + " degrees Celsius is equal to " + fahrenheit.toFixed(2) + " degrees Fahrenheit";
    }
    
    function convertToFahrenheit() {
      var fahrenheit = parseFloat(document.getElementById("celsiusInput").value);
      var celsius = (fahrenheit - 32) * 5/9;
      document.getElementById("result").innerHTML = fahrenheit + " degrees Fahrenheit is equal to " + celsius.toFixed(2) + " degrees Celsius";
    }
  </script>
  <hr>
  <footer>
    <div>
    <h3>Temperature Converter</h3>
    <h4>
    -by atharv sonare
    </h4>
    </div>
  </footer>
</body>
</html>
