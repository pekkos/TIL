[Source](https://superuser.com/questions/1245704/got-an-error-on-apche-localhost-configtest)

/var/log/apache2 should exist on macOS as it comes with its own Apache server. If it does not you could try to create it yourself again by doing:

```bash
sudo mkdir /var/log/apache2 && sudo chown root:wheel /var/log/apache2
```


[More tricks](https://apple.stackexchange.com/questions/351031/i-can-t-connect-to-localhost-on-mac-high-sierra]
