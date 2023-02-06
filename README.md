### John Kantlehner Z23474365
---
<p align = "center">
    <img src = https://github.com/cop4808-spring-2023-fullstack-web/cop4808-git-and-github-fundamentals-jkantlehner2018/blob/main/calculator.gif alt = "calculator gif" >
</p>
---
## Buttons Added 


| Button | Description | 
| ----------- | ----------- |
| e<sup>x<sup> | operation |
| √ (sqrt) | operation |
| π | operand |
| x<sup>y<sup>| operation |


---
- ### Handling for New Buttons
```
            else if(buttons[i].classList.contains('e')) {
                  inputE(displayValue);
                  updateDisplay();
            }
            else if(buttons[i].classList.contains('sqrt')) {
                  inputSqrt(displayValue);
                  updateDisplay();
            }
            else if(buttons[i].classList.contains('pi')) {
                  inputOperand(Math.PI.toFixed(9));
                  updateDisplay();

            }
            else if(buttons[i].classList.contains('exponent')) {
                  inputOperator(buttons[i].value);
            }
```
- ### Functions added for single operand operations
```
            function inputE(num) {
                displayValue = Math.exp(num).toString();
            }

            function inputSqrt(num) {
                displayValue = Math.sqrt(num).toString();
            }
```
- ### Exponent operation added in operate function
```
        
            else if(op === 'exponent'){
                return Math.pow(x,y);
            }
```
---
