# Clear the "Open with..." Finder option from duplicates
http://mac-how-to.wonderhowto.com/how-to/remove-duplicates-customize-open-with-menu-mac-os-x-0157100/

```bash
$ /System/Library/Frameworks/CoreServices.framework/Frameworks/LaunchServices.framework/Support/lsregister -kill -r -domain local -domain system -domain user
````

```
$ killall Finder
```
