# pointer-events

The pointer-events property may be used for some interesting hover effects, like preventing a parent hover style from taking effect until an enclosed button is hovered. 


Read more about it here: [CSS pointer-events: clever hover states](https://medium.com/@erinannette/css-pointer-events-simple-clever-hovers-with-just-a-few-lines-of-code-d44a14a4e06f).

And check [this codepen](https://codepen.io/MartijnCuppens/full/MBjqbM/) out.

[Can I use?](https://caniuse.com/#feat=pointer-events)

```
.parent {
  pointer-events: none;
  
  &:hover {
    background-color: #c0ffee;
  }
}

.btn {
  // All btns are clickable/hoverable
  pointer-events: auto;
}
```
