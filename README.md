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
default: ```<value>``` = ```flex-start```: items are aligned to the left\
```<value>``` = ```flex-end```: items aligned to the right\
```<value>``` = ```center```: items will be centered.\
```<value>``` = ```space-around```: leftover space will be used as a margin between items, equally distributed\
```<value>``` = ```space-between```: same as ```space-around```, but with none on the outer edges of the first/last elements
```
justify-content: <value>
```
default: ```<value>``` = ```row```: items stack left to right\
```<value>``` = ``` ```
```
flex-flow: <value>

---

### items
default: ```<value>``` = ```0```: no growth\
when applied to items, they will expand into available width.\
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
if ```flex-grow``` isn't enabled, this will be their max width\
if ```flex-shrink``` is disabled, this will be their minimum width
```
flex-basis: <value>
```
a shorthand method to define ```flex-grow```, ```flex-shrink``` and ```flex-basis``` all at once\
if a single ```<value>``` is presented, it will be used to define the ```flex-grow```and ```flex-shrink```. ```flex-basis``` will be untouched\
default: ```<value>``` = ```0```
```
flex: <flex-grow> <flex-shrink> <flex-basis>
```
