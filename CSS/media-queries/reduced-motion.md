# Reduced motion preference
If a user preferes reduced motion in MacOS/iOS, use this trick to calculate the duration with motion on or off:

[Source](https://twitter.com/steveg3003/status/888500276847562752)

Markup:

```html
<a href="#">Hover me</a>
<p>Moveable</p>
```

CSS:

```css
:root {
  --motion: 1;
}

@media (prefers-reduced-motion: reduce) {
  :root {
    --motion: 0;
  }
}

p {
  transition: transform .3s ease-in-out;
  transition-duration: calc(var(--motion) * .3s);
}

a:hover + p {
  transform: translateY(100px);
}
```

[Lab example](http://lab.pekkos.com/reduced-motion.html)


