# Variables in CSS / Custom Properties

## 🌟Intro

CSS variables are a new addition that works the same as variables in any language where you store some data and reference it by the variable name later in the code.

*Previously this feature was one of the things that made CSS preprocessors famous but now it is natively available in CSS to be used without any setup*

Now same in CSS you can store different CSS property values and then use them in with respective CSS properties.

**Now let's see how to define and use CSS variables:**

### 🌟Defining the Variable:

```css
   --var-name: value;
```

As you can see you need to start the variable name with a double `dash(-)` and use the kabab case for the variable name then `colon(:)` and finally the value you want to store

Ex:

```css
   --background-color : Lightblue;
```

Now comes the topic of where to define the variable, because you'll need a scope for variables and in HTML/CSS the elements are the scope.

Ex:

```css
.container{
    --background-color: black;
}
```

now all the elements in this element with container class can access the background color variable.

The best practice here would be to define all variables in the `:root` scope. Because in the HTML document it is the root of the element tree or parent element of all elements in HTML, so this way you will have access to variables in the whole CSS file.

### 🌟Using the variable:

After defining the variable it's just a matter of using it and here's how you do it,

Ex:

```css
element {
    background: var(--background-color);
}
```

As seen in the example whenever you want to use the custom property/variable you write it inside `var()` and that's it.

This way you can nearly save any property in a variable and reference the variable name without typing it.

This comes in very handy when is a style change or some component upgrade where you'd have to go and find those properties and change them one by one, and in this case, you just change the values where you defined variable and that's it, the change will be reflected all over CSS.

* * *

**If you found the content I share useful then share it with your developer friends and also follow me on** [Instagram](https://www.instagram.com/gaurav_vaala/) **and** [Twitter](https://twitter.com/gaurav_vaala)