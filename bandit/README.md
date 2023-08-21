<h1 align="center">Bandit Cheetsheet | OverTheWire</h1>

<h3>Level 0</h3>

* username: `bandit0`
* password: `bandit0`
* hostname: `bandit.labs.overthewire.org`
* port: `2220`

**SSH:** `ssh -p 2220 bandit0@bandit.labs.overthewire.org`

After you've gained the shell, `cat` the readme file, which contains the password for `bandit1.

---

<h3>Level 1</h3>

* username: `bandit1`
* password: `NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL` *(password might be changed in future)*
* hostname: `bandit.labs.overthewire.org`
* port: `2220`

**SSH:** `ssh -p 2220 bandit1@bandit.labs.overthewire.org`

If you `ls` the directory you can see that there is a file named `-`. Since it's a special character in bash you can't directly print the content of this file by using `cat -` but if you specify absolute path you can just like that:

```bash
cat "`pwd`/-"
```

The content is the password for `bandit2`, now you can go to next level.

---

<h3>Level 2</h3>

* username: `bandit2`
* password: `rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi` *(password might be changed in future)*
* hostname: `bandit.labs.overthewire.org`
* port: `2220`

**SSH:** `ssh -p 2220 bandit2@bandit.labs.overthewire.org`

if you `ls -la`, you can see that there is a file with spaces, since it has some spaces you can't directly specify the filename for `cat` command but you can either use `\` to escape whitespaces or use `"` just like that:

* `cat spaces\ in\ this\ filename`
* `cat "spaces in this filename"`

After you've printed the content of this file, you should be good to proceed to the next level.

---



