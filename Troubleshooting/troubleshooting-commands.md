# **Troubleshooting Master List**

# OSI Model

### Layer 1



### Layer 2
Ping
 
apr -a
show arp

**windows**

ipconfig

**Linux**

ifconfig


### Layer 3
nslookup



### Layer 4


### Layer 5


### Layer 6


### Layer 7





# HTTP Status Errors
### Most Common

**400s (400,401,404)**

<u>You (client) did something wrong.</u>

**500s (500, 502, 504)**

<u>They(server) did something wrong.</u>



# Searching in Linux
```
$ find 

$ find .
 ```
 'find' works like ls, it will list  all files in current directory and those in sub directories. sometimes requires '.'

 ```
$ find / 
 ```
 searches everying from the rood folder down

 ```
$ find / -name "*.*s"
$ find . -name "*.?s"

$ find / -name "*.pem"

$ find / -name '*.js"
 ```
The thee commands are different examples of using linux find command.
1) will search for every file from the root folder down that have  extention name with with *=any charachter then  s (c.css, yelp.js, highlight.pack.js)
2) is the same command but only searched the current folder and will only return 2 letter extentsions (yelp.js, highlight.pack.js)

3) this command will search everything from the root folder down that is a pem file
4) this command will only return js files
 