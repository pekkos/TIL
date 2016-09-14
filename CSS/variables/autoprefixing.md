## Autoprefixing

The clever [Lea Verou shows us a way to autoprefix](http://lea.verou.me/2016/09/autoprefixing-with-css-variables/) using CSS variables.

```
* {
	--clip-path: initial;
	-webkit-clip-path: var(--clip-path);
	clip-path: var(--clip-path);
}

header {
	--clip-path: polygon(0% 0%, 100% 0%, 100% calc(100% - 2.5em), 0% 100%);
}
```

<cite>Even !important should work, because it affects the cascading of CSS variables. Furthermore, if for some reason you want to explicitly set -webkit-clip-path, you can do that too, again because * has zero specificity.</cite>
