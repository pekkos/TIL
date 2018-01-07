# display: flow-root;

Block formatting context may be created by using display: flow-root;

A good explanation of [BFC by Rachel Andrew](https://www.smashingmagazine.com/2017/12/understanding-css-layout-block-formatting-context/) here.

Current [browser support for display: flow-root](https://caniuse.com/#feat=flow-root).

Using it together with @supports seems to be a good way forward, even if it adds a few extra lines of CSS.

```
.overflow {
  overflow: auto;
}

@supports (display: flow-root) {
  display: flow-root;
  overflow: initial;
}
```
