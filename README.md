html structure
```
<flex-container>
  <flex-item>
  <flex-item>
</flex-container>
```

---

### container
turn an element into a flex container.\
```
display: flex
```
default: ```<value>``` = ```nowrap```: when a minimum width is reached, items will start to go off the page\
<value>``` = ```wrap```: the last item(s) will be pushed below\
```<value>``` = ```reverse```: the last item(s) will be pushed above. all items will then expand to fill the new, free space\
```
flex-wrap: <value>
```
default: ```<value>``` = ```flex-start```: items are aligned to the start\
```<value>``` = ```flex-end```: items aligned to the end\
```<value>``` = ```center```: items will be centered.\
```<value>``` = ```space-around```: leftover space will be used as a margin between items, equally distributed\
```<value>``` = ```space-between```: same as ```space-around```, but with none on the outer edges of the first/last elements
```
justify-content: <value>
```
  if ```<value>``` is changed from a horizontal (like ```row```) to a vertical (like ```column```), the main and cross axis will be inverted\
default: ```<value>``` = ```row```: items stack left to right\
```<value>``` = ```column```: items stack top to bottom\
  ```<value>``` = ``````:
```
flex-flow: <value>
```

---

### items
default: ```<value>``` = ```0```: no growth\
when applied to items, they will expand into available space (main axis)\*\
```<value>``` is used to determine how much items will grow in relation to eachother\
an item with a ```<value>``` of 2 will grow twice as fast as an item with a ```<value>``` of 1
```
flex-grow: <value>
```
the opposite of ```flex-grow```\
default: ```<value>```  = 1: items will shrink at the same rate\
the higher the ```<value>```, the more an item will shrink
```
flex-shrink: <value>
```
defines the starting size of an item\
if ```flex-grow``` isn't enabled, this will be their max size (main axis)\*\
if ```flex-shrink``` is disabled, this will be their min size (main axis)\*
```
flex-basis: <value>
```
a shorthand method to define ```flex-grow```, ```flex-shrink``` and ```flex-basis``` all at once\
if a single ```<value>``` is presented, it will be used to define the ```flex-grow```and ```flex-shrink```. ```flex-basis``` will be untouched\
```
flex: <flex-grow> <flex-shrink> <flex-basis>
```

---

\* depending on which direction is chosen as the main axis (determined by ```flex-flow```), this value could apply to the horizontal or vertical
