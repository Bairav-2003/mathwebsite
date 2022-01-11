# Web Page for Mathematical Calculations

## AIM:

To design a static website with validation to perform mathematical calculations in client side.

## DESIGN STEPS:

### Step 1:

Requirement collection.

### Step 2:

Creating the layout using HTML and CSS.

### Step 3:

Write javascript to perform the calculations.

### Step 4:

Include regularexpression based input validation.

### Step 5:

Validate the layout in various browsers.

### Step 6:

Validate the HTML code.

### Step 6:

Publish the website in the given URL.

## PROGRAM :
~~~ html
<!DOCTYPE html>
<html lang="en">
  
<head>
    <title>Loan Calculator</title>
  
    <style>
        body {
            background-color: yellow;
            font-family: 'Trebuchet MS';
        }
          
        h1 {
            font-size: 35px;
        }
          
        h1 {
            font-size: 21px;
            margin-top: 20px;
        }
          
        .calculator {
            width: 400px;
            height: 450px;
            background-color: black;
            position: absolute;
            left: 50%;
            top: 50%;
            transform: translateX(-50%) translateY(-50%);
            padding: 20px 0px 0px 100px;
            color: white;
        }
          
        input {
            padding: 7px;
            width: 70%;
            margin-top: 7px;
        }
    </style>
</head>
  
<body>
    <div class="calculator">
        <h1>Loan Calculator</h1>
  
        <p>Amount  :
            <input id="amount" type="number" 
            onchange="Calculate()">
        </p>
  
        <p>Interest Rate  :
            <input id="rate" type="number" 
            onchange="Calculate()">
        </p>
  
        <p>Months to Pay :
            <input id="months" type="number" 
            onchange="Calculate()">
        </p>
  
        <h2 id="total"></h2>
    </div>
  
<script>
function Calculate() {
  const amount = document.getElementById("amount").value;
  const rate = document.getElementById("rate").value;
  const months = document.getElementById("months").value;
  const interest = (amount * (rate * 0.01)) / months; 
  const total = ((amount / months) + interest).toFixed(2);
  document.getElementById("total").innerHTML = "EMI : (₹)" + total;
}  
</script>
</body>
  
</html>
~~~ 
## OUTPUT:
![](e1.png)

## Result:

Thus a website is designed to perform mathematical calculations in the client side.
