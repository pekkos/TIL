# Clear the "Open with..." Finder option from duplicates

My Finder option menu gets cluttered with duplicates of apps in different versions, here is a way to clear the menu.

```bash
$ /System/Library/Frameworks/CoreServices.framework/Frameworks/LaunchServices.framework/Support/lsregister -kill -r -domain local -domain system -domain user
````

```
$ killall Finder
```

[Source](http://mac-how-to.wonderhowto.com/how-to/remove-duplicates-customize-open-with-menu-mac-os-x-0157100/)
