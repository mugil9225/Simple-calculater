<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculator</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
        }

        .calculator {
            background: #2d3748;
            border-radius: 20px;
            padding: 25px;
            box-shadow: 0 20px 60px rgba(0, 0, 0, 0.4);
            width: 320px;
        }

        .display {
            background: #1a202c;
            border-radius: 12px;
            padding: 20px;
            margin-bottom: 20px;
            min-height: 80px;
            display: flex;
            flex-direction: column;
            justify-content: flex-end;
            align-items: flex-end;
            word-wrap: break-word;
            word-break: break-all;
        }

        .previous-operand {
            color: #a0aec0;
            font-size: 1.2rem;
            min-height: 1.5rem;
        }

        .current-operand {
            color: #ffffff;
            font-size: 2rem;
            font-weight: 600;
            min-height: 2.5rem;
        }

        .buttons {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 12px;
        }

        button {
            border: none;
            border-radius: 10px;
            font-size: 1.3rem;
            padding: 20px;
            cursor: pointer;
            transition: all 0.2s;
            font-weight: 600;
            outline: none;
        }

        button:hover {
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
        }

        button:active {
            transform: translateY(0);
        }

        .number {
            background: #4a5568;
            color: #ffffff;
        }

        .number:hover {
            background: #5a6578;
        }

        .operator {
            background: #ed8936;
            color: #ffffff;
        }

        .operator:hover {
            background: #f59642;
        }

        .operator.active {
            background: #f59642;
            box-shadow: 0 0 0 2px #ffffff;
        }

        .clear {
            background: #fc8181;
            color: #ffffff;
            grid-column: span 2;
        }

        .clear:hover {
            background: #ff8a8a;
        }

        .delete {
            background: #f6ad55;
            color: #ffffff;
        }

        .delete:hover {
            background: #ffb866;
        }

        .equals {
            background: #48bb78;
            color: #ffffff;
            grid-column: span 2;
        }

        .equals:hover {
            background: #5cc889;
        }

        .zero {
            grid-column: span 2;
        }

        .keyboard-hint {
            text-align: center;
            color: #ffffff;
            font-size: 0.85rem;
            margin-top: 15px;
            opacity: 0.7;
        }
    </style>
</head>
<body>
    <div class="calculator">
        <div class="display">
            <div class="previous-operand" id="previousOperand"></div>
            <div class="current-operand" id="currentOperand">0</div>
        </div>
        <div class="buttons">
            <button class="clear" onclick="calculator.clear()">AC</button>
            <button class="delete" onclick="calculator.delete()">DEL</button>
            <button class="operator" onclick="calculator.chooseOperation('÷')">÷</button>
            
            <button class="number" onclick="calculator.appendNumber('7')">7</button>
            <button class="number" onclick="calculator.appendNumber('8')">8</button>
            <button class="number" onclick="calculator.appendNumber('9')">9</button>
            <button class="operator" onclick="calculator.chooseOperation('×')">×</button>
            
            <button class="number" onclick="calculator.appendNumber('4')">4</button>
            <button class="number" onclick="calculator.appendNumber('5')">5</button>
            <button class="number" onclick="calculator.appendNumber('6')">6</button>
            <button class="operator" onclick="calculator.chooseOperation('-')">−</button>
            
            <button class="number" onclick="calculator.appendNumber('1')">1</button>
            <button class="number" onclick="calculator.appendNumber('2')">2</button>
            <button class="number" onclick="calculator.appendNumber('3')">3</button>
            <button class="operator" onclick="calculator.chooseOperation('+')">+</button>
            
            <button class="number zero" onclick="calculator.appendNumber('0')">0</button>
            <button class="number" onclick="calculator.appendNumber('.')">.</button>
            <button class="equals" onclick="calculator.compute()">=</button>
        </div>
        <div class="keyboard-hint">Keyboard shortcuts supported</div>
    </div>

    <script>
        class Calculator {
            constructor(previousOperandElement, currentOperandElement) {
                this.previousOperandElement = previousOperandElement;
                this.currentOperandElement = currentOperandElement;
                this.clear();
            }

            clear() {
                this.currentOperand = '0';
                this.previousOperand = '';
                this.operation = undefined;
                this.shouldResetScreen = false;
                this.updateDisplay();
            }

            delete() {
                if (this.currentOperand === '0') return;
                if (this.currentOperand.length === 1) {
                    this.currentOperand = '0';
                } else {
                    this.currentOperand = this.currentOperand.slice(0, -1);
                }
                this.updateDisplay();
            }

            appendNumber(number) {
                if (this.shouldResetScreen) {
                    this.currentOperand = '';
                    this.shouldResetScreen = false;
                }
                
                if (number === '.' && this.currentOperand.includes('.')) return;
                
                if (this.currentOperand === '0' && number !== '.') {
                    this.currentOperand = number;
                } else {
                    this.currentOperand += number;
                }
                
                this.updateDisplay();
            }

            chooseOperation(operation) {
                if (this.currentOperand === '') return;
                
                if (this.previousOperand !== '') {
                    this.compute();
                }
                
                this.operation = operation;
                this.previousOperand = this.currentOperand + ' ' + operation;
                this.shouldResetScreen = true;
                this.updateDisplay();
            }

            compute() {
                let computation;
                const prev = parseFloat(this.previousOperand);
                const current = parseFloat(this.currentOperand);
                
                if (isNaN(prev) || isNaN(current)) return;
                
                switch (this.operation) {
                    case '+':
                        computation = prev + current;
                        break;
                    case '−':
                        computation = prev - current;
                        break;
                    case '×':
                        computation = prev * current;
                        break;
                    case '÷':
                        if (current === 0) {
                            alert('Cannot divide by zero!');
                            this.clear();
                            return;
                        }
                        computation = prev / current;
                        break;
                    default:
                        return;
                }
                
                this.currentOperand = this.formatNumber(computation);
                this.operation = undefined;
                this.previousOperand = '';
                this.shouldResetScreen = true;
                this.updateDisplay();
            }

            formatNumber(number) {
                const stringNumber = number.toString();
                if (stringNumber.length > 12) {
                    return parseFloat(number.toPrecision(12)).toString();
                }
                return stringNumber;
            }

            updateDisplay() {
                this.currentOperandElement.textContent = this.currentOperand;
                this.previousOperandElement.textContent = this.previousOperand;
            }
        }

        // Initialize calculator
        const previousOperandElement = document.getElementById('previousOperand');
        const currentOperandElement = document.getElementById('currentOperand');
        const calculator = new Calculator(previousOperandElement, currentOperandElement);

        // Keyboard support
        document.addEventListener('keydown', (e) => {
            // Numbers
            if (e.key >= '0' && e.key <= '9') {
                calculator.appendNumber(e.key);
            }
            
            // Decimal point
            if (e.key === '.' || e.key === ',') {
                calculator.appendNumber('.');
            }
            
            // Operations
            if (e.key === '+') {
                calculator.chooseOperation('+');
            }
            if (e.key === '-') {
                calculator.chooseOperation('−');
            }
            if (e.key === '*') {
                calculator.chooseOperation('×');
            }
            if (e.key === '/') {
                e.preventDefault(); // Prevent browser search
                calculator.chooseOperation('÷');
            }
            
            // Equals
            if (e.key === 'Enter' || e.key === '=') {
                calculator.compute();
            }
            
            // Clear
            if (e.key === 'Escape' || e.key.toLowerCase() === 'c') {
                calculator.clear();
            }
            
            // Delete
            if (e.key === 'Backspace' || e.key === 'Delete') {
                calculator.delete();
            }
        });

        // Visual feedback for keyboard presses
        document.addEventListener('keydown', (e) => {
            const key = e.key;
            let buttonText;
            
            if (key === '*') buttonText = '×';
            else if (key === '/') buttonText = '÷';
            else if (key === '-') buttonText = '−';
            else if (key === 'Enter') buttonText = '=';
            else if (key === 'Escape' || key.toLowerCase() === 'c') buttonText = 'AC';
            else if (key === 'Backspace' || key === 'Delete') buttonText = 'DEL';
            else buttonText = key;
            
            const buttons = document.querySelectorAll('button');
            buttons.forEach(button => {
                if (button.textContent === buttonText) {
                    button.style.transform = 'translateY(0)';
                    setTimeout(() => {
                        button.style.transform = '';
                    }, 100);
                }
            });
        });
    </script>
</body>
</html>
