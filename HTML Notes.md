# Useful snippets of HTML

 Tells the browser to always fetch the latest version of the page from the server rather than using a stored copy. 
 This can be especially useful for dynamic pages or content that frequently changes.

 ```html
<meta http-equiv="cache-control" content="no-cache">
```

SVG's an in depth look at them:

The <symbol> element is used to declare a graphic (or part of one) that can be reused later. However, by itself, a <symbol> does not render anything on the screen—it’s just a definition or a “template.”
The <use> element tells the browser to instantiate or "use" the previously defined symbol with the id "logo". This is what actually renders the graphic on the page. Without the <use> element, the symbol would remain just a definition and nothing would be displayed.
 ```html
<?xml version="1.0" encoding="UTF-8"?>
<svg version="1.0"
  xmlns="http://www.w3.org/2000/svg">
  <symbol id="logo" viewBox="0 0 60 60">
    <!-- Your graphic elements like <path> and <rect> -->  </symbol>
  <use href="#logo" />   THIS LINE USES THE SVG
</svg>
```
