# Ex.08 Design of a Standard Calculator
## Date:21-12-2023

## AIM:
To design a web application for a standard calculator with minimum five operations.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for creating attractive colors.

### Step 4:
Write JavaScript program for implementing five different operations.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
``` 
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculator</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }

        #calculator-container {
            background-color:red;
            text-align: center;
            border: 1px solid #12121200;
            padding: 20px;
            border-radius: 10px;
        }

        input {
            width: 85%;
            padding: 10px;
            margin: 5px 0;
        }

        button {
            width: 50px;
            height: 48px;
            font-size: 16px;
            margin: 5px;
        }
    </style>
</head>
<body>
    <div id="calculator-container">
        <h2><font color= "white"></fontcolor>Gedipudi Darshani</h2>
        <h3>212223230062</h3>
        <h2>CALCULATOR</h2>

        <input type="text" id="display" disabled>

        <br>
	<button onclick="appendToDisplay('(')">(</button>
	<button onclick="appendToDisplay(')')">)</button>
	<button onclick="appendToDisplay('.')">.</button>
    <button onclick="apprndToDisplay('+')">+</button>
	
            
 	<br>

       
        <button onclick="appendToDisplay('7')">7</button>
        <button onclick="appendToDisplay('8')">8</button>
        <button onclick="appendToDisplay('9')">9</button>
        <button onclick="appendToDisplay('-')">-</button>
	
        

        <br>

        <button onclick="appendToDisplay('4')">4</button>
        <button onclick="appendToDisplay('5')">5</button>
        <button onclick="appendToDisplay('6')">6</button>
        <button onclick="appendToDisplay('*')">*</button>
        

        <br>
	
        <button onclick="appendToDisplay('1')">1</button>
        <button onclick="appendToDisplay('2')">2</button>
        <button onclick="appendToDisplay('3')">3</button>
        <button onclick="appendToDisplay('/')">/</button>

        
	<br>
    <button onclick="calculate()">=</button>
    <button onclick="appendToDisplay('0')">0</button>
	
    <button onclick="clearDisplay()">C</button>
    <button onclick="appendToDisplay('%')">%</button>
    </div>

    <script>
        function clearDisplay() {
            document.getElementById('display').value = '';
        }

        function appendToDisplay(value) {
            document.getElementById('display').value += value;
        }

        function calculate() {
            try {
                document.getElementById('display').value = eval(document.getElementById('display').value);
            } catch (error) {
                document.getElementById('display').value = 'Error';
            }
        }
    </script>
</body>
</html>


```

## OUTPUT:


![Alt text](<darshani/cal/static/Screenshot (216).png>)


![Alt text](<darshani/cal/static/Screenshot (217).png>)







## RESULT:
The program for designing a standard calculator using HTML and CSS is executed successfully.
