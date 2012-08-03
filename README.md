MathematiCSS!
=============

MathematiCSS is a CSS preprocessor written in JavaScript that allows you to use delicious math expressions, functions, and variables in your style sheets. Why? Well just 'cause.

What kind of features does MathematiCSS offer? Currently, MathematiCSS allows you to crunch numbers in any chunk of a css rule. The functions it currently accepts are:

* **exp(x)**, find the result of raising e (Euler's number) to any value x;
* **log(x)**, calculate the natural logarithm of x, or use log(x)/log(y) to find the value of logy(x);
* **sqrt(x)**, find those squares;
* **pow(x,y)**, determine the value of x^y;
* **abs(x)**, the absolute value function;
* **sin(x)**, and the other trigonometric function, as well as their sweet inverses;
* **pi()**, gives you pi to more digits than you would ever type out by hand, trust me.

MathematiCSS has just started so you should expect to see many more features in the near future!

Getting Started With MathematiCSS
-----------------------

Installing and using MathematiCSS is a piece of cake. All you need is the mathematicss.js JavaScript code and a couple of keystrokes.

You can write MathematiCSS rules in your website's main CSS file, or you can write a separate styles sheet, it's up to you!

Start off by including mathematicss.js in your HTML file:

```html
	<script src="mathematicss.js" type="text/javascript"></script>
```

Then, include all CSS files with MathematiCSS rules between the `<head>` tags of your HTML file, as you would a normal style sheet. The only difference is that you need to add "/mathematicss" to the relation attribute of your tag, like so:

```html
	<link rel="stylesheet/mathematicss" type="text/css" href="general.css" />
```

The next step is to write your first lines of MathematiCSS rules. You'll probably find that doing this is pretty easy and intuitive. All MathematiCSS expressions need to be enclosed with `math(...)`. Check out the examples:

```css
body{
	background: -webkit-linear-gradient(top, #fff math(log(1)), #BBB 100%);
	box-shadow: inset 0 0 math(10*pi()/2)px rgba(105,212,255,1);
	height:100%;
	margin:math(pow(4,2)/8-2);
	width:100%;
}
```

MathematiCSS gives you the ability to create variables in your CSS so that you can reuse the same values multiple times. To declare a variable, preface your variable name with an '@' symbol and give it a value like: `@mywidth: 50;`. Variables must start with a letter, but after that can be alphanumeric. They need a `:` after the variable name and a `;` after the variable value. You can declare variables anywhere in your sheet, however to keep your CSS pretty, you might want to declare them at the top. The coolest thing about variables is that you can use math functions in your variable definitions. Check this out:

```css
@marginleft: math(2*30/7);

p{
	background-color: #math(23*12);
	margin-left: @marginleft%;
}

a{
	margin-left: math(0.5*@marginleft)%
}

```

Stay tuned!

-[lsvx](https://twitter.com/lsvx)
