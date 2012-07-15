MathematiCSS!
-------------

MathematiCSS is a CSS preprocessor written in JavaScript that allows you to use delicious math expressions and functions in your style sheets. Why? Well just 'cause.

What kind of features does MathematiCSS offer? Currently, MathematiCSS allows you to crunch numbers in any chunk of a css rule. The functions it currently accepts are:

* **exp(x)**, find result of raising e (Euler's number) to any value x;
* **log(x)**, calculate the natural logarithm of x, or use log(x)/log(y) to find the value of logy(x);
* **sqrt(x)**, find those squares;
* **pow(x,y)**, determine the value of x^y;
* **pi()**, gives you pi to more digits than you would ever type out by hand, trust me.

MathematiCSS has just started so you should expect to see many more features in the near future!

Getting Started With MathematiCSS
-----------------------

Installing and using MathematiCSS is a piece of cake. All you need is the mathematicss.js JavaScript code and a couple of keystrokes.

You can write MathematiCSS rules in your websites main CSS file, or you can write a separate CSS file, it's up to you.

Start off by including mathematicss.js in your HTML file:

```html
	<script src="mathematicss.js" type="text/javascript"></script>
```

Then include all CSS files with MathematiCSS rules between the <head> tags of your HTML file, as you would a normal style sheet. The only difference is that you need to add "/mathematicss" to the relation attribute of your tag, like so:

```html
	<link rel="stylesheet/mathematicss" type="text/css" href="general.css" />
```

The next step is to wite your first lines of MathematiCSS rules. You'll probably find that doing this is pretty easy and intuitive. All MathematiCSS expressions need to be enclosed with math(...). Check out the examples:

```css
body{
	background: -webkit-linear-gradient(top, #fff math(log(1)), #BBB 100%);
	box-shadow: inset 0 0 math(10*pi()/2)px rgba(105,212,255,1);
	height:100%;
	margin:math(pow(4,2)/8-2);
	width:100%;
}
```

Stay tuned!

-lsvx
