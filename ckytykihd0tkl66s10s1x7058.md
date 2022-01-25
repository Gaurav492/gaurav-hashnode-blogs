## How to use Local fonts in CSS

There are many great fonts that you might want to use into your website but that font might not be a font which you can import to your CSS file like you can do with some like google fonts.

Importing local font into CSS is a little different than importing fonts from websites like Google fonts, where we have import at-rule (@import) 

Example:

```
@import url('https://fonts.googleapis.com/css?family=Open+Sans&display=swap');
```

_You might have seen this syntax where we just pass the font URL._

___

## Importing local font

Now, to import a local/downloaded font into your css file there is a different CSS at-rule that creates a custom font property that you can reference in your css file.

```
@font-face 
{ 
font-family: "Open Sans";  
src: url("/fonts/OpenSans-Regular-webfont.woff2")format("woff2"); 
}
```

This a simple and clear syntax at first look, you are giving a name to reference your font `font-family:`, also giving the the relative URL to your font `src:` and the format of the font `format`

You can use same syntax again for different styles of same font like bold or light.

Here, you can use any name in the font-family, and reference that name in css afterwards, so different names for different styles.

Also, It would be a good practice that you create a fonts folder in your assets folder to store the font.

_ For reference and more detailed overview you can check out section of MDN on same here -> [MDN Link](https://developer.mozilla.org/en-US/docs/Web/CSS/@font-face)_

___

** If you found the content i share useful than share it with your developer friends and also follow me on [Instagram](https://www.instagram.com/gaurav_vaala/) and [Twitter](https://twitter.com/gaurav_vaala) **
