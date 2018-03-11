html structure
```
<flex-container>
  <flex-item>
  <flex-item>
</flex-container>
```

---

### container
turn an element into a flex container
```
display: flex
```
determines the direction in which items will stack and which axis are the main/cross\
default: ```<value>``` = ```row```: items stack left to right, aligned to the left\
```<value>``` = ```column```: items stack top to bottom, aligned to the top\
```<value>``` = ```row-reverse```: items will start right to left, aligned to the right\
```<value>``` = ```column-reverse```: items stack bottom to top, aligned to the bottom\
```
flex-direction: <value>
```
default: ```<value>``` = ```nowrap```: when a minimum width is reached, items will start to go off the page\
```<value>``` = ```wrap```: the last item(s) will be pushed below\
```<value>``` = ```reverse```: the last item(s) will be pushed above. all items will then expand to fill the new, free space
```
flex-wrap: <value>
```
a shorthand for setting ```flex-direction```and ```flex-wrap```
  ```
  flex-flow: <flex-direction> <flex-wrap>
  ```
```justify-content``` applies to the main axis\*\
default: ```<value>``` = ```flex-start```: items are aligned to the start\
```<value>``` = ```flex-end```: items aligned to the end\
```<value>``` = ```center```: items will be centered.\
```<value>``` = ```space-around```: leftover space will be used as a margin between items, equally distributed\
```<value>``` = ```space-between```: same as ```space-around```, but with none on the outer edges of the first/last elements
```
justify-content: <value>
```
```align-items``` applies to the cross axis\*\

```
align-items: <value>
```

---

### items
when applied to items, they will expand into available space (main axis)\*\
default: ```<value>``` = ```0```: no growth\
```<value>``` is used to determine how much items will grow in relation to eachother\
an item with a ```<value>``` of 2 will grow twice as fast as an item with a ```<value>``` of ```1```
```
flex-grow: <value>
```
the opposite of ```flex-grow```\
default: ```<value>```  = 1: items will shrink at the same rate\
the higher the ```<value>```, the more an item will shrink
```
flex-shrink: <value>
```
defines the starting size of an item on the main axis \*\
```flex-grow``` = 0: ```<value>``` will be their max size\
```flex-shrink``` = 0: ```<value>``` will be their min size\
```
flex-basis: <value>
```
a shorthand for setting ```flex-grow```, ```flex-shrink``` and ```flex-basis```\
if a single ```<value>``` is presented, it will be used to define the ```flex-grow```and ```flex-shrink```. ```flex-basis``` will be untouched
```
flex: <flex-grow> <flex-shrink> <flex-basis>
```

---

\* depending on which direction is chosen as the main axis (determined by ```flex-direction```), this value could apply to the horizontal or vertical
