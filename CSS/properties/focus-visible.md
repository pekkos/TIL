# focus-visible

The pseudo-selector :focus-visible will be implemented in browsers, and with it comes the possibility to style :focus when navigated to by keyboard, but keep it unseen when navigated to using mouse/pointer.

Read more about it here: [:focus-visible and backwards compatibility](https://developer.paciellogroup.com/blog/2018/03/focus-visible-and-backwards-compatibility/).

[Can I use?](https://caniuse.com/#search=%3Afocus-visible)

```
button:focus { /* some exciting button focus styles */ }
button:focus:not(:focus-visible) {
    /* undo all the above focused button styles
       if the button has focus but the browser wouldn't normally
       show default focus styles */
}
button:focus-visible { /* some even *more* exciting button focus styles */ }
```
