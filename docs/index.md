
<html>
    <head>
      
      
      
      <style>
      
      body,html {
    color: black;
    display:block;
    width:100%;
    margin:0;
    padding:0;
}
form {
    background-color: pink;
    display: inline-block;
    box-sizing: border-box;
    box-shadow: 2px 2px 20px 5px black;
    margin: 0;
    padding: 10px;
    width:100%;
    max-width: 400px;
}
input {
    box-shadow: 1px 1px 3px 1px black;
    width: 100%;
    text-align: center;
}

.submit {
    display:inline-block;
    color: white;
    background-color: blue;
    margin:0;
    padding: 5px;
    border: 0;
    font-weight: bold;
    width:100%;
}
.submit:hover {
    color: blue;
    background-color: white;
    font-size: 0.7em;
    font-weight: bold;
}

#result {
    border: 1px solid black;
    padding: 2px;
    color: white;
    width: 100%;
    text-align: center;
}

h4 {
    color: black;
    text-shadow: -2px -2px 5px white;
    
}



      
      
      </style>
        <title>BMI Calculator</title>
        <meta name="viewport" content="width=device-width,initial-scale=1">
    </head>
    <body>
        <form>
            <h4>BMI Calculator</h4>
            <input id="weight" type="text" placeholder="Your weight in kilograms" />
            <br />
            <br />
            <input id="height" type="text" placeholder="Your height in meters" />
            <br />
            <br />
            
            <input class = "submit" type="button"  value="Submit" onclick="bmi()" />
            <p id="result">Here will be your result</p>
        </form>
    </body>
</html>

<script>
function bmi () {
var height = Number(document.getElementById("height").value);
var weight = Number(document.getElementById("weight").value);
var result = weight / (height * height);
document.getElementById("result").innerHTML = "Your bmi score is : " + result;
}


</script>
