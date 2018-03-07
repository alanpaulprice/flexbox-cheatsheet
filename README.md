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
by default, items will stack left to right and the container will span full width
```
display: flex
```
when a minimum width is reached, by default (```<value>``` of ```nowrap```), the items will start to go off the page\
```<value>``` of ```wrap```, the last item(s) will be pushed below\
```<value>``` of ```reverse```, the last item(s) will be pushed above\
all items will then expand to fill the new, free space\
```
flex-wrap: <value>
```

---

### items
by default, ```<value>``` is ```0``` (no growth)\
when applied to items, they will expand into available width.\
```<value>``` is used to determine how much items will grow in relation to eachother\
(an item with a ```<value>``` of 2 will grow twice as fast as an item with a ```<value>``` of 1)
```
flex-grow: <value>
```
the opposite of ```flex-grow```. by default, items will shrink at the same rate\
the higher the ```<value>```, the more it will shrink
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
if a single ```<value>``` is presented, it will be used to define the ```flex-grow```and ```flex-shrink```. ```flex-basis``` will be left at a default ```<value>``` of ```0```.
```
flex: <flex-grow> <flex-shrink> <flex-basis>
```
