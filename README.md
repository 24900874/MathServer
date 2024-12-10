# Ex.05 Design a Website for Server Side Processing
## Date:8.12.2024

## AIM:
 To design a website to calculate the power of a lamp filament in an incandescent bulb in the server side. 


## FORMULA:
P = I<sup>2</sup>R
<br> P --> Power (in watts)
<br> I --> Intensity
<br> R --> Resistance

## DESIGN STEPS:

### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Create python programs for views and urls to perform server side processing.

### Step 5:
Create a HTML file to implement form based input and output.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lamp Filament Power Calculator</title>
    <style>
        /* Global Styles */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f0f0f0;
        }

        header {
            background-color: #333;
            color: #fff;
            padding: 20px;
            text-align: center;
        }

        main {
            margin: 20px;
            text-align: center;
        }

        section.calculator {
            background-color: #fff;
            border-radius: 8px;
            padding: 20px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            display: inline-block;
            width: 300px;
            text-align: left;
        }

        label {
            display: block;
            margin: 10px 0 5px;
            font-weight: bold;
        }

        input {
            margin-bottom: 10px;
            padding: 8px;
            width: calc(100% - 16px);
            box-sizing: border-box;
            border: 1px solid #ccc;
            border-radius: 4px;
        }

        button {
            padding: 10px 20px;
            background-color: #333;
            color: #fff;
            border: none;
            cursor: pointer;
            border-radius: 4px;
            width: 100%;
            font-size: 1em;
            font-weight: bold;
        }

        button:hover {
            background-color: #555;
        }

        #result {
            margin-top: 20px;
            font-size: 1.2em;
            color: #333;
            padding: 10px;
            background-color: #e0e0e0;
            border-radius: 4px;
            text-align: center;
        }

        footer {
            background-color: #333;
            color: #fff;
            text-align: center;
            padding: 10px;
            position: fixed;
            bottom: 0;
            width: 100%;
        }
    </style>
</head>
<body>
    <header>
        <h1>Lamp Filament Power Calculator</h1>
    </header>
    <main>
        <section class="calculator">
            <h2>Enter Values to Calculate Power</h2>
            <form id="powerForm">
                <label for="intensity">Intensity (I):</label>
                <input type="number" id="intensity" name="intensity" required>
                
                <label for="resistance">Resistance (R):</label>
                <input type="number" id="resistance" name="resistance" required>
                
                <button type="button" onclick="calculatePower()">Calculate Power</button>
            </form>
            <div id="result"></div>
        </section>
    </main>
    <footer>
        <p>&copy; Geethapriyan A S </p>
    </footer>

    <script>
        function calculatePower() {
            var intensity = document.getElementById('intensity').value;
            var resistance = document.getElementById('resistance').value;
            
            if (intensity && resistance) {
                var power = Math.pow(intensity, 2) * resistance;
                document.getElementById('result').innerHTML = '<strong>Power (P):</strong> ' + power.toFixed(2) + ' watts';
            } else {
                document.getElementById('result').innerText = 'Please enter both Intensity and Resistance';
            }
        }
    </script>
</body>
</html>


```


## SERVER SIDE PROCESSING:

![image](https://github.com/user-attachments/assets/9a9663ca-2c3c-46e1-8cb6-36ee2d657ece)




## HOMEPAGE:
![image](https://github.com/user-attachments/assets/ba27746c-c511-4cd5-a79b-f2594c6f106b)



## RESULT:
The program for performing server side processing is completed successfully.
