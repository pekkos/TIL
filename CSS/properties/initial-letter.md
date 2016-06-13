# initial-letter for drop caps

Drop caps can be made using a combination of initial-letter property and the ::first-letter pseudo element.

A [tutoriel here](http://webdesign.tutsplus.com/tutorials/better-css-drop-caps-with-initial-letter--cms-26350).

The margin-top value is there to prevent the first line to spill over the edge of the container.

```
h1 + p:first-of-type::first-letter {
  @supports (initial-letter: 3) or (-webkit-initial-letter: 3) {
    -webkit-initial-letter: 3;
    initial-letter: 3;
    margin-top: 1em;
    margin-right: .5em;
    color: #9a1a1a;
  }
}
```
