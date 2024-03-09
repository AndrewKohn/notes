---
created:
  - 2024-03-09 10:43
tags:
  - html
---
# Hyperlinks

Links that point to our own pages within our website:
```
 <a href="blog.html">BLOG</a>
```

Links that point to outside of our website:
```
    <p>
      You can learn more at the
      <a href="https://developer.mozilla.org/en-US/docs/Web/HTML"
        >MDN Web Docs</a
      >.
    </p>
```
"a" is the anchor element and "href" is the attribute which contains the hyperlink.  Notice the difference in the href attribute between href's.

The hyperlink can open to a new tab by:
```
    <p>
      You can learn more at the
      <a
        href="https://developer.mozilla.org/en-US/docs/Web/HTML"
        target="_blank"				//the "_blank" target attribute allows the link to be opened asap.
        >MDN Web Docs</a
      >.
    </p>
```

The hyperlink can be created without it pointing to anywhere yet:
```
	<a href="blog.html">BLOG</a>				//all three links with actual addresses will have a link
	<a href="adfasdf.html">adfasdf</a>		
	<a href="adsfege.html">adsfege</a>
	<a href="#">BLOG</a>						//a link is created, but will do nothing.
```