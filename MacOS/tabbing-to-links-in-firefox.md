# Tabbing to links in Firefox

It's a Mac problem. Mozilla is being true to operating system settings in Mac OS.

There are two distinct ways around this on the user side. Both seem to work:

In System Preferences → Keyboard, in the Shortcuts pane, check the “all controls” radio at the bottom.

In Firefox, type "about:config" in the URL bar. There is no accessibility.tabfocus preference on the mac, so you'll have to make one. Right click in the window, create a new "integer" pref, and set it to 7.

Neither of these are terribly obvious. Also, neither of these are a server-side solution for developers, which is frustrating.

Source: [https://stackoverflow.com/questions/11704828/how-to-allow-keyboard-focus-of-links-in-firefox](https://stackoverflow.com/questions/11704828/how-to-allow-keyboard-focus-of-links-in-firefox)
