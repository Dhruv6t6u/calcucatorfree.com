<!DOCTYPE html>
<html>
<style type="text/css">
body{
  background-color:#f5f5f5;
  padding:0;
  margin:0;
  background-color: #151845;
}
.mycanvas{
  height:370px;
  width:370px;
  position:absolute;
  margin:auto;
  left:0;
  right:0;
  top:0;
  bottom:0;
}
.details{
  background-color:white;
  height:7%;
  width:100%;
  position:absolute;
  bottom:0;
  display:flex;
  align-items:center;
  justify-content:space-around;
}
.details>a{
  text-decoration:none;
  display:block;
  color:#000066;
  font-size:150%;
}
.moon{
  background-color: #39BEFF;
  height: 170px;
  width: 170px;
  border-radius: 50%;
  position: absolute;
  margin: auto;
  top:0;
  bottom: 0;
  left: 0;
  right: 0;
  overflow: hidden;
}
.crater{
  background-color:#31B4FF;
  height: 30px;
  width: 30px;
  border-radius: 50%;
  position: relative;
}
.crater:before{
  content: "";
  position: absolute;
  height: 25px;
  width: 25px;
  border:none;
  border-radius: 50%;
  box-shadow: -5px 0 0 2px #1CA4F9;
  top:2px;
  left: 7px;
}
.c1{
  top:27px;
  left: 90px;
  transform: scale(0.9);
  -webkit-transform: scale(0.9);
}
.c2{
  transform: scale(0.6);
  -webkit-transform: scale(0.6);
  bottom:15px;
  left: 61px;
}
.c3{
  transform: scale(0.75);
  -webkit-transform: scale(0.75);
  left: 15px;
}
.c4{
  transform: scale(1.18);
  -webkit-transform: scale(1.18);
  left: 107px;
  top:32px;
}
.c5{
  transform: scale(0.67);
  -webkit-transform: scale(0.67);
  left: 33px;
  bottom:4px;
}
.shadow{
  height: 190px;
  width: 190px;
  box-shadow: 21px 0 0 5px rgba(0,0,0,0.15);
  border-radius: 50%;
  position: relative;
  bottom: 157.5px;
  right:46px; 
}
.eye{
  height: 12px;
  width: 12px;
  background-color: #161646;
  border-radius: 50%;
  position: relative; 
}
.el{
  bottom: 255px;
  left: 59px;
}
.er{
  bottom: 267px;
  left: 101px;
}
.mouth{
  height: 5px;
  width: 10px;
  position: relative;
  border:3px solid #161646;
  border-top:none;
  bottom: 262px;
  left: 79px;
  border-radius: 0 0 10px 10px;
}
.blush{
  height: 7.5px;
  width: 7.5px;
  background-color:#1CA4F9;
  position: relative;

  border-radius: 50%;
}
.b1{
  bottom: 273px;
  left: 50px;
}
.b2{
  bottom: 281px;
  left: 115px;
}
.orbit{
  height: 280px;
  width: 280px;
  border-radius: 50%;
  position: absolute;
  margin: auto;
  top:0;
  bottom: 0;
  left: 0;
  right: 0;
  animation:rotate 5s infinite linear;
  -webkit-animation:rotate 5s infinite linear;
}
@keyframes rotate{
  100%{
    transform: rotate(360deg);
  }
}
@-webkit-keyframes rotate{
  100%{
    -webkit-transform: rotate(360deg);
  }
}
.rocket{
  background-color: #FAFCF7;
  height: 50px;
  width: 25px;
  border-radius: 50% 50% 0 0;
  position: relative;
  left: -11px;
  top:115px;

}

.rocket:before{
  position: absolute;
  content: "";
  background-color:  #f6f6f6;
  height: 20px;
  width: 55px;
  right: -15px;
  border-radius: 50% 50% 0 0;
  bottom: 0;
  z-index: -1;
}
.rocket:after{
  position: absolute;
  content: "";
  background-color:  #39BEFF;
  height: 4px;
  width: 15px;
  border-radius: 0 0 2px 2px;
  bottom: -4px;
  left: 4.3px;
}
.window{
  height: 10px;
  width: 10px;
  background-color: #151845;
  border:2px solid #B8D2EC;
  border-radius: 50%;
  position: relative;
  top:17px;
  left: 5px;
}
/* Created By Terrance*/
*
{
   margin:0; 
   padding:0;
   box-sizing:border-box;
}    

body
{
    display:flex;
    justify-content:center;
    align-items:center;
    min-height:100vh;
    background:#091921;
}

.calculator
{
   position:relative; 
   display:grid;
}

.calculator .value
{
    grid-column:span 4;
    height:100px;
    text-align:right;
    border:none;
    outline:none;
    padding:10px;
    font-size:18px;
}

.calculator span
{
    display:grid;
    width:90px;
    height:90px;
    color:#fff;
    background:#0c2835;
    place-items:center;
    border:1px solid rgba(0,0,0,.1);
}

.calculator span:active
{
    background:#74ff3b;
    color:#111;
}

.calculator span.clear
{
    grid-column:span 2;
    width:180px;
    background:#ff3077;
}

.calculator span.plus
{
    grid-row:span 2;
    height:180px;
}

.calculator span.equal
{
    background:#03b1ff;
}








</style>
    <head>
        <title>Calculator</title>
    </head>
    <body>
        <form class="calculator" name="calc">
            <input class="value" type="text" name="txt" readonly="">
            <span class="num clear" onclick="document.calc.txt.value =''">C</span>
            <span class="num" onclick="document.calc.txt.value +='/'">/</span>
            <span class="num" onclick="document.calc.txt.value +='*'">*</span>
            <span class="num" onclick="document.calc.txt.value +='7'">7</span>
            <span class="num" onclick="document.calc.txt.value +='8'">8</span>
            <span class="num" onclick="document.calc.txt.value +='9'">9</span>
            <span class="num" onclick="document.calc.txt.value +='-'">-</span>
            <span class="num" onclick="document.calc.txt.value +='4'">4</span>
            <span class="num" onclick="document.calc.txt.value +='5'">5</span>
            <span class="num" onclick="document.calc.txt.value +='6'">6</span>
            <span class="num plus" onclick="document.calc.txt.value +='+'">+</span>
            <span class="num" onclick="document.calc.txt.value +='3'">3</span> 
            <span class="num" onclick="document.calc.txt.value +='2'">2</span>
            <span class="num" onclick="document.calc.txt.value +='1'">1</span>
            <span class="num" onclick="document.calc.txt.value +='0'">0</span> 
            <span class="num" onclick="document.calc.txt.value +='00'">00</span>
            <span class="num" onclick="document.calc.txt.value +='.'">.</span>
            <span class="num equal" onclick="document.calc.txt.value = eval(calc.txt.value)">=</span>
        </form>
    </body>
</html>
  
