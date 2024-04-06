---
title: HTML
tags:
  - 前端学习
  - 编程
categories: 前端开发
keywords: [HTML ,前端 ,编程]
top_img: >-
  https://img1.baidu.com/it/u=1360347520,1922694507&fm=253&fmt=auto&app=138&f=JPEG?w=889&h=500
cover: >-
  https://img1.baidu.com/it/u=3046825186,2319338927&fm=253&fmt=auto&app=138&f=JPEG?w=500&h=729
abbrlink: 2eec1551
date: 2024-04-06 19:08:34
---
# HTML
![计算机](/IMG/calm.png)
### 计算机小案例
```HTML
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
  <style>
    body {
      background-color: #f2f2f2;
      font-family: Arial, sans-serif;
    }
    
    .container {
      margin: auto;
      margin-top: 100px;
      width: 300px;
      padding: 10px;
      border: 1px solid #ccc;
      background-color: #fff;
      box-shadow: 0px 0px 10px #ccc;
    }
    
    .output {
      font-size: 2em;
      text-align: right;
      padding: 10px;
      background-color: #eee;
      border: 1px solid #ccc;
    }
    
    .button {
      font-size: 1.5em;
      margin: 5px;
      width: 50px;
      height: 50px;
      border: none;
      background-color: #ccc;
      color: #fff;
      cursor: pointer;
    }
    
    .button:hover {
      background-color: #999;
    }
    
    .clear {
      background-color: #ff6666;
    }
    
    .equals {
      background-color: #66cc66;
    }
</style>
</head>
<body>
  <div class="container">
    <div class="output" id="output">0</div>
    <button class="button" onclick="clearOutput()" id="clear">C</button>
    <button class="button" onclick="appendToOutput('%')">%</button>
    <button class="button" onclick="appendToOutput('/')">/</button>
    <button class="button" onclick="appendToOutput('*')">*</button>
    <button class="button" onclick="appendToOutput('7')">7</button>
    <button class="button" onclick="appendToOutput('8')">8</button>
    <button class="button" onclick="appendToOutput('9')">9</button>
    <button class="button" onclick="appendToOutput('-')">-</button>
    <button class="button" onclick="appendToOutput('4')">4</button>
    <button class="button" onclick="appendToOutput('5')">5</button>
    <button class="button" onclick="appendToOutput('6')">6</button>
    <button class="button" onclick="appendToOutput('+')">+</button>
    <button class="button" onclick="appendToOutput('1')">1</button>
    <button class="button" onclick="appendToOutput('2')">2</button>
    <button class="button" onclick="appendToOutput('3')">3</button>
    <button class="button equals" onclick="calculate()">=</button>
    <button class="button" onclick="appendToOutput('0')">0</button>
    <button class="button" onclick="appendToOutput('.')">.</button>
</div>

<script>
  let output = document.getElementById("output");
  
  function appendToOutput(value) {
    if (output.innerHTML === "0") {
      output.innerHTML = value;
    } else {
      output.innerHTML += value;
    }
  }
  
  function clearOutput() {
    output.innerHTML = "0";
  }
  
  function calculate() {
    output.innerHTML = eval(output.innerHTML);
  }
</script>
</body>
</html>





```
