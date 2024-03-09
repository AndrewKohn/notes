---
created:
  - 2024-03-09 10:39
tags:
  - css
---
# Flexbox

Flexbox is generally easier to work with than floats in CSS.  
```
        /* FLEXBOX */
        display: flex;
        align-items: center;
        justify-content: space-between;
```

![[flexbox-1.png]]

-----

- The main idea behind flexbox is that empty space inside a container element can be automatically divided by its child elements
- makes it easy to automatically align items to one another.
- Flexbox solves common problems such as vertical centering and creating equal-height columns.
- Flexbox is perfect for replacing floats, allowing us to write fewer and cleaner HTML/CSS code.

---

### Flexbox terminology

![[flexbox-2.png]]

![[flexbox-3.png]]

---

##### Flex property
```
Default setting for the flex properties:
 flex-grow: 0;

 flex-shrink: 1;

 flex-basis: auto;
```

Adding properties is not absolute.  Think of it as giving the browser recommendations to create the dimension.

```
 flex: 0 0 200;  			//shorthand version of the three usages above
 
 flex: [flex-grow] [flex-shrink] [flex-basis];
```
