# :lang pseudo class

Use the :lang pseudo-class to add styling based on language.

The :lang pseudo-class is used to select an element based on its content language. The content language of an element is determined by a combination of three things:

- Any lang attributes
- Meta tags, e.g. <meta http-equiv="content-language" content="en">
- HTTP headers, e.g. Content-language: en

This means that the :lang pseudo-class can be used even in cases where no lang attribute is specified.
Block formatting context may be created by using display: flow-root;



Read the whole [article by Ire Aderinokun](https://bitsofco.de/use-the-lang-pseudo-class-over-the-lang-attribute-for-language-specific-styles/) here.

Current [browser support for :lang](https://caniuse.com/#search=%3Alang).

```
p:lang(es) {
  background-color: yellow;
  color: #000;
}
```

