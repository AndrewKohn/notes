---
created:
  - 2024-03-09 10:52
tags:
  - html
---
# Text elements

Heading Example:
```
<!DOCTYPE html>
<html>
  <head>
    <title>The Basic Language of the web: HTML</title>
  </head>

  <body>
    <h1>The Basic Language of the web: HTML</h1>
    <h2>The Basic Language of the web: HTML</h2>
    <h3>The Basic Language of the web: HTML</h3>
    <h4>The Basic Language of the web: HTML</h4>
    <h5>The Basic Language of the web: HTML</h5>
    <h6>The Basic Language of the web: HTML</h6>
  </body>
</html>
```

# The Basic Language of the web: HTML
## The Basic Language of the web: HTML
### The Basic Language of the web: HTML
#### The Basic Language of the web: HTML
##### The Basic Language of the web: HTML
###### The Basic Language of the web: HTML

----

HTML code commenting:
```
<!-- COMMENTED CODE WILL NOT APPEAR HERE -->		//Single line

  <body>											//Multi line
    <h1>The Basic Language of the web: HTML</h1>
    <h2>The Basic Language of the web: HTML</h2>
    <h3>The Basic Language of the web: HTML</h3>
    <!--
	<h4>COMMENTED CODE WILL NOT APPEAR HERE</h4>
    <h5>COMMENTED CODE WILL NOT APPEAR HERE</h5>	
    <h6>COMMENTED CODE WILL NOT APPEAR HERE</h6>	
    -->
  </body>
```

---

Bolding text:
```
<b>TEXT</b>		//Will bold text characters.
```
This element is not preferred as it is just an element that doesn't mean anything.  It is preferred to use the "strong" element to also bold a selected piece of text, but also give meaning that the selected text is an important element we would want to stand out on the page.

```
<strong>TEXT</strong>	//Will bold text characters and is better practice.
```

---

Italicizing text:
```
<i>TEXT</i>		//Will italicize characters.
```
Same idea as the bolding concept above, this "i" element doesn't give much meaning.  "em" is preferred as it gives the text meaning as it is "em"phasized.  Thus, it's preferred to use:
```
<em>TEXT</em>		//Will italicize characters and is better practice.
```

---

Ordered List:
```
<ol>
	<li>The opening tag</li>
	<li>The closing tag</li>
	<li>The actual element</li>
</ol>
```

![[text-el-1.png]]

Defined as "ol", an ordered list (essentially like a container) has a child element "li" within it that let's the browser render this ordered list as a list of numbers.  It is automatically numbered and anything inserted on top of the list will take the first index and shift every other part of the list downward.

```
<ul>
      <li>To be able to use the fundamental web dev language</li>
      <li>
        To hand-craft beautiful websites instead of relying on tools like
        Worpress or Wix
      </li>
      <li>To build web applications</li>
      <li>To impress friends</li>
      <li>To have fun 😃</li>
</ul>
```

![[text-el-2.png]]

"ul" element refers to "Unordered List" element.  Within that unordered list, the "li" element is still used.  The code above will output a bullet point list within a webpage.
