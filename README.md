# TryHackMe: Thompson

---

By: *UnknownPerson*

---

nmap -sC -sV -Pn -vv {IP}

## Port Scanning: {22,8000}

```
This web page containing the pyrat programm which simple work is to netcat login and performing shell command 
in this it have vurnability that thro basic command line connection like
telnet , nc we can directly access this script and throw 
shell we get basic www-data shell
```

## Intial Access

shell
--

```
We got our basic shell let's travers in all directory 
Woow look at this in /opt/dev/.git/config file have password of user
think
```
think:_TH1N***GPi***e$_
--

## Privillage Escallation

```
We try evrything but we dont get any way to get root shell 
than i read blog post of ctf challange throw that i get to know that in this throw telnet ot nc basic 
connection we have to pass many username throw that some one have direct login access
so we try some that using fuzzing trick and user name was "admin"

Than same thing we have to fuzz about passowrd asnd throw that we alos get password 
```

admin:a**1*3
--

As this way we agin Pawned New machine {Thompson}
--