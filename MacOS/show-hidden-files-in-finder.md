

# Show hidden files in Finder

Open Terminal and type the following to show hiddden files in Finder.

```bash
$ defaults write com.apple.finder AppleShowAllFiles YES
````

Now, relaunch Finder by holding alt/option while right clicking the Finder icon; select Relaunch from the Finder menu.


To hide hidden files again, type the following, and relaunch Finder afterwards,

```bash
$ defaults write com.apple.finder AppleShowAllFiles NO
```

Note to self: I have followed the instructions in the source and created the aliases showFiles and hideFiles respectively.

[Source](http://ianlunn.co.uk/articles/quickly-showhide-hidden-files-mac-os-x-mavericks/)
