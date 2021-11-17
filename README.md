# calculater
Hi, I want to make a calculator with css and html. This is a hobby. You will see many other things later. Thanks


html.............................................................................................
<form class="calculator" name="calc">
        <input type="text" class="value" name="txt" readonly="">
        <span class="num clare" onclick="document.calc.txt.value += ''">c</span>
        <span class="num" onclick="document.calc.txt.value += '/'">/</span>
        <span class="num" onclick="document.calc.txt.value += '*'">*</span>
        <span class="num" onclick="document.calc.txt.value += '7'">7</span>
        <span class="num" onclick="document.calc.txt.value += '8'">8</span>
        <span class="num" onclick="document.calc.txt.value += '9'">9</span>
        <span class="num" onclick="document.calc.txt.value += '-'">-</span>
        <span class="num" onclick="document.calc.txt.value += '4'">4</span>
        <span class="num" onclick="document.calc.txt.value += '5'">5</span>
        <span class="num" onclick="document.calc.txt.value += '6'">6</span>
        <span class="num plus" onclick="document.calc.txt.value += '+'">+</span>
        <span class="num" onclick="document.calc.txt.value += '3'">3</span>
        <span class="num" onclick="document.calc.txt.value += '2'">2</span>
        <span class="num" onclick="document.calc.txt.value += '1'">1</span>
        <span class="num" onclick="document.calc.txt.value += '0'">0</span>
        <span class="num" onclick="document.calc.txt.value += '00'">00</span>
        <span class="num" onclick="document.calc.txt.value += '.'">.</span>
        <span class="num lal" onclick="document.calc.txt.value = eval(calc.txt.value)">=</span>

  
  
  
  css..............................................................................................
     * {
        padding: 0px;
        margin: 0px;
        box-sizing: border-box;
        font-family: Tahoma, sans-serif;
    }
    
    body {
        display: flex;
        justify-content: center;
        min-height: 100vh;
        align-items: center;
        background-color: darkslateblue;
    }
    
    .calculator {
        position: relative;
        display: grid;
    }
    
    .value {
        grid-column: span 4;
        height: 100px;
        outline: none;
        border: none;
        padding: 10px;
        font-size: 18px;
        color: black;
    }
    
    .calculator span {
        display: grid;
        width: 60px;
        height: 60px;
        color: #fff;
        background: #0c2835;
        place-items: center;
        border: 1px solid rgba(0, 0, 0, .1);
    }
    
    .calculator span:active {
        background-color: springgreen;
    }
    
    .calculator span.clare {
        grid-column: span 2;
        width: 120px;
        background: rgb(240, 65, 161);
    }
    
    .calculator span.plus {
        grid-row: span 2;
        height: 120px
    }
    
    .calculator span.lal {
        background: #1e8cbe;
    }
