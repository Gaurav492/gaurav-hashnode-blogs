## Where to put the script tag?

## Intro 

While using External JavaScript file there are 2 ways by which you can attach the file to html document

1. In the head tag
1. Befor body tag is closed

Now ** according to how you attached your javascript file in html document, it may behave differently ** like html tag not getting selected.

** The preferred way of attaching js file is to _ add to end, before the body tag is closed _, let's see why. **

## Why use it at end?

The index html file in your project will be executed first in the project and there a hierarchy of html elements will be created which will be executed top to bottom. 

### Attaching it in head tag

When you attach your js file in the head tag the js file will be running before your html is rendered and that means whenever you'll be trying select an element in javascript it will give error because that element is not rendered and javascript file can't find it. _ It is like using a variable before it was defined. _


### Attaching it before body tag is closed

So when you attach your js file at the end of the document, every element will be rendered first and at last the javascript file will be executed and that means it will have access to every element in your html document.

> There are ways to make it work perfectly even after attaching it into head tag, but personally i feel like this is more cleaner way.

___

** If you found the content i share useful than share it with your developer friends and also follow me on [Instagram](https://www.instagram.com/gaurav_vaala/) and [Twitter](https://twitter.com/gaurav_vaala) **