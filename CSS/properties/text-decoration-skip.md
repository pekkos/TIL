# text-decoration-skip

Make underlines stay behind descending glyphs by using text-decoration-skip.

A few resources on the subject:

[text-decoration-skip on MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/text-decoration-skip)

[text-decoration-skip on CSS Tricks](https://css-tricks.com/almanac/properties/t/text-decoration-skip/)

Also a sibling property:
[text-decoration-skip-ink on MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/text-decoration-skip-ink)

**Note**

*ink* seems to be a valid value in Chrome Developer Tools, but the MDN spec don't list *ink* as a property value.

Found [a note](https://github.com/openstyles/stylus/issues/229) about that here:

*Chrome 57 introduced text-decoration-skip: ink to skip glyph descenders for text-decoration: underline.
CSS committee decided to use a separate property text-decoration-skip-ink: auto.
Chrome 64 removed the old property entirely and enabled the new one by default.

This is Chrome-specific as Firefox hasn't yet implemented ink skipping.
I think we should revisit this issue in a year or so (November 2018) and probably remove text-decoration-skip: ink from our pages.*

```
a {
  text-decoration: underline;
  text-decoration-skip: ink;
}
```
