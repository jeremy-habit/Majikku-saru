# Monkey-Zero

## What ?

Monkey-Zero is a CSS library offering practical classes and a responsive grid based on Flexbox. You can check for the documentation inside the folder documentation.

## Install with NPM or YARN

Monkey-Zero can be installed thanks to [NPM](https://www.npmjs.com/) ( <https://www.npmjs.com/package/magic-monkey> ) :

```bash
npm i magic-monkey
```

or

```bash
#if yarn is not installed on your computer
npm i -g yarn

# add magic-monkey to your project
yarn add magic-monkey
```


## Import with Webpack

You can import the style sheet in your javascript file :



### ES6

```js
import 'monkey-zero'
```



### CommonJS

```js
require('monkey-zero')
```



## Reset CSS

I invite you to use a CSS reset such as [Normalize.css](https://necolas.github.io/normalize.css/) ( there are others, I let you make your choice  ). Why use a CSS reset ? It's simply because every web browser applies diffrent CSS properties by default to HTML tags.

Let us admit that the web browser Google Chrome applies 15 pixels of margin on the \<p> tag againt 10 pixels for the web browser Firefox (it's not a real example). In this case, the CSS reset will overload these default values and thus  applies the same value of margin to the <\p> tag no matter the web browser.

To resume,  your web application will almost present no more differences of display no matter the web browser used by the user. It's worth it !

## Organization : adopt an architecture

It is frequent and easy to get lost about style sheets in an important Web application. To avoid or only to limit the probabilities to get lost, I recommend you to adopt an architecture in which you can fast find the style sheet which includes such or such CSS rules.

There is no perfect architecture to my knowledge but this following one is pretty cool : [the 7-1 Pattern](https://gist.github.com/rveitch/84cea9650092119527bc)

I think there is one important criterion in order to respect an architecture pattern : it is the DISCIPLINE ! Indeed, don't break the rules of your architecture. Even if it's a question of adding quickly a small CSS rule, write this last one where it has to be and not in the first style sheet at hand. Otherwise, you will continue to make this kind of breach for the rule and will increase the risks of losing you in a disorder...
   

## License

MIT