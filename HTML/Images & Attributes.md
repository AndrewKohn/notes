---
created:
  - 2024-03-09 10:45
tags:
  - html
  - programming
---
# Images & Attributes

Image element:
```
	<img src="post-img.jpg"/>
		//img = element
		//src="blah.jpg" = attribute
```
![[img-attributes-1.png]]

Unlike the other elements, img elements don't have a "/img" ending.
	Within the "img" element, the "src" (source) is the attribute that is describing the element.
There are other attributes other than "src", such as "alt" (alternative text), which describes what the image is about.  This is important as it allows search engines to understand what the image is actually about.  Just as important, if not more important:  By describing the imaging, it allows blind people to use a website and understand what that image is trying to convey.  Also, if the "src" path is incorrect or nonexistant, the "alt" text will be shown and can help identify what the image is suppose to show.
```
	<img src="post-img.jpg" alt="HTML code on a computer monitor"/>			//Correct
	<img src="post-img.jp" alt="HTML code on a computer monitor"/>			//Incorrect
\	
```
![[img-attributes-2.png]]

```
    <img												//Formatting of an img element
      src="post-img.jpg"									//Source attribute
      alt="HTML code on a computer monitor"					//Alternative Text attribute
      width="500"											//Width attribute
      height="200"											//Height attribute
    />
```

![[img-attributes-3.png]]

Attributes can be assigned to other elements as well, like:
```
<html lang="en">
```
Which in this example indicates this html is set for English speaking persons.