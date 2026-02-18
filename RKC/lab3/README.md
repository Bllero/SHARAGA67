# ТРЕНИРОВКА С EMMET

## ЗАДАНИЕ 1. Подберите максимально краткое сокращение Emmet

## Структура 1:
```html
<div class="logo"> <a href=""><img src="" alt=""></a> <nav> <a href=""></a> <a href=""></a> <a href=""></a> </nav> </div>
```
Сокращение: .logo>a>img^nav>a*3
Пояснение: .logo - div с классом logo; > - вложенность; a>img - ссылка с картинкой внутри; ^ - подняться на уровень вверх; nav>a*3 - навигация с тремя ссылками

Структура 2:
```html
<h2></h2> <h2></h2> <div class="comment"> <img src="" alt="" class="comment_foto"> <div class="comment_text"></div> </div>
```
Сокращение: h2*2+.comment>img.comment_foto+.comment_text
Пояснение: h2*2 - два заголовка; + - соседний элемент; .comment - div с классом comment; img.comment_foto - картинка с классом; +.comment_text - соседний div с классом

Структура 3:
```html
<form action=""> <select name="" id=""> <option value=""></option> <option value=""></option> </select> <input type="date"> <input type="date"> <input type="number"> <select name="" id=""> <option value=""></option> <option value=""></option> </select>
```
Сокращение: form>select>option*2^^input:date*2+input:number+select>option*2
Пояснение: form>select>option*2 - форма с select и двумя option; ^^ - подняться на два уровня вверх; input:date*2 - два поля с типом date; +input:number - поле с типом number; +select>option*2 - еще один select с двумя option

## ЗАДАНИЕ 2. Расшифруйте сокращения Emmet

Сокращение: h1+div.steps>div.step*6
Результат:
```html 
<h1></h1>
<div class="steps">
    <div class="step"></div>
    <div class="step"></div>
    <div class="step"></div>
    <div class="step"></div>
    <div class="step"></div>
    <div class="step"></div>
</div>
```
Сокращение: h1+nav>a*7
Результат:
```html
<h1></h1>
<nav>
    <a href=""></a>
    <a href=""></a>
    <a href=""></a>
    <a href=""></a>
    <a href=""></a>
    <a href=""></a>
    <a href=""></a>
</nav>
```
Сокращение: div.promo>img+h2+div.promo_text+button
Результат:
```html
<div class="promo">
    <img src="" alt="">
    <h2></h2>
    <div class="promo_text"></div>
    <button></button>
</div>
```
Сокращение: div.info>h2+p*2+p>ul>li*3^^p*3
Результат:
```html
<div class="info">
    <h2></h2>
    <p></p>
    <p></p>
    <p>
        <ul>
            <li></li>
            <li></li>
            <li></li>
        </ul>
    </p>
    <p></p>
    <p></p>
    <p></p>
</div>
```