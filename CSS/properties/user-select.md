# user-select for easier text selection

Inputs have selection boundaries, meaning you can click into them and (for example) Select All and get just the text inside the input.

There is a CSS property that allows us to do that without needing to use a not-particularly-semantically-appropriate form input.

An [overview here](https://css-tricks.com/force-selection-text-block/).

```
.force-select-all {
  -webkit-user-select: all;
  -moz-user-select: all;
  -ms-user-select: all;
  user-select: all;
}
```
