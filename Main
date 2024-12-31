```html
<!DOCTYPE html>
<html>
<head>
    <title>Calculadora Completa Online</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: white; /* Cor de fundo padrão */
            color: black; /* Cor do texto padrão */
        }
        #display {
            width: 100%;
            height: 40px;
            font-size: 24px;
            background-color: lightblue; /* Cor de fundo do display */
            border: none;
        }
        button {
            width: 25%;
            height: 50px;
            font-size: 20px;
            background-color: white; /* Cor de fundo dos botões */
            border: 1px solid lightblue; /* Borda dos botões */
            cursor: pointer;
        }
        button:hover {
            background-color: lightblue; /* Efeito ao passar o mouse */
        }
        .dark-mode {
            background-color: black; /* Cor de fundo no modo escuro */
            color: white; /* Cor do texto no modo escuro */
        }
        .dark-mode #display {
            background-color: gray; /* Cor do display no modo escuro */
        }
        .dark-mode button {
            background-color: black; /* Cor de fundo dos botões no modo escuro */
            border: 1px solid white; /* Borda dos botões no modo escuro */
        }
    </style>
</head>
<body>

<h1>Calculadora Completa Online</h1>
<input type="text" id="display" readonly>

<div>
    <button onclick="appendNumber('7')">7</button>
    <button onclick="appendNumber('8')">8</button>
    <button onclick="appendNumber('9')">9</button>
    <button onclick="appendOperator('+')">+</button>
</div>
<div>
    <button onclick="appendNumber('4')">4</button>
    <button onclick="appendNumber('5')">5</button>
    <button onclick="appendNumber('6')">6</button>
    <button onclick="appendOperator('-')">-</button>
</div>
<div>
    <button onclick="appendNumber('1')">1</button>
    <button onclick="appendNumber('2')">2</button>
    <button onclick="appendNumber('3')">3</button>
    <button onclick="appendOperator('*')">*</button>
</div>
<div>
    <button onclick="appendNumber('0')">0</button>
    <button onclick="appendOperator('/')">/</button>
    <button onclick="calculate()">=</button>
    <button onclick="clearDisplay()">C</button>
</div>
<div>
    <button onclick="toggleDarkMode()">Modo Escuro</button>
</div>

<script>
    let display = document.getElementById("display");
    let currentInput = "";
    let darkMode = false;

    function appendNumber(number) {
        currentInput += number;
        display.value = currentInput;
    }

    function appendOperator(operator) {
        currentInput += operator;
        display.value = currentInput;
    }

    function calculate() {
        try {
            display.value = eval(currentInput) || "Erro";
            currentInput = display.value;
        } catch (error) {
            display.value = "Erro";
        }
    }

    function clearDisplay() {
        currentInput = "";
        display.value = "";
    }

    function toggleDarkMode() {
        darkMode = !darkMode;
        document.body.classList.toggle("dark-mode", darkMode);
    }
</script>

</body>
</html>
```
