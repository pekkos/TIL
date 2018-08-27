# Flexbox with auto margins

Turns out that auto margins on flex items can do magic, like aligning an item differently than the other items.

```css 

.parent {
  display: flex;
  justify-content: flex-start;
}

.child:last-child {
  margin-left: auto;
}
```

The above would align the last child all the way to the right, despite justify-content tells all items to line up starting from the left.


Read [this article](https://css-tricks.com/the-peculiar-magic-of-flexbox-and-auto-margins/) on css-tricks, and [this one by Sam Provenza](https://hackernoon.com/flexbox-s-best-kept-secret-bd3d892826b6).

![](https://cdn-images-1.medium.com/max/800/1*RPnezwYfOsZcTq8u7a5-ew.png)
