# Change default Terminal prompt

1. Navigate to your home directory:

```bash
$ cd ~
```

2. Create a file called .bash_profile:

```bash
$ vi .bash_profile
```

3. Add the following line (press i):

```bash
export PS1="\W $ "
```

4. Save the file with esc, type :wq and enter

5. Restart Terminal

6. You should now see the working directory followed by a $ prompt

[Source](https://mattmazur.com/2012/01/27/how-to-change-your-default-terminal-prompt-in-mac-os-x-lion/)
