CTFGames


#OverTheWire


Passwords

=======
=======


0
```
      Had to download putty and enter host and port
```

1. boJ9jbbUNNfktd78OOpsqOltutMc3MY1
```
      In order to find file named - I had to type ./- with cat
```

2. CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9
```
      Had to cat with "spaces in this filename"
```

3. UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK
```
      cd inhere
```

4. pIwrPrtPN36QITSp3EQaw936yaFoFgAB
```
	I went into each file in inhere and found it using cat and ls
```

5. koReBOKuIDDepwhWk7jZC0RTdopnAYKh
```		
	  Went into inhere then searched for a file with 1033 bytes by using find -size 1033c
```	   
6. DXjZPULLxYr17uwoI01bNLQbtFemEgo7
```
	used different searching tools such as -user -size and -group
```
7. HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs
```
	Grep prints lines, different type of find tool, looks for patterns
	used grep millionth
```
8.  cvX2JJa4CFALtqS87jk27qwqGhBM9plV
```
	Uniq removes repeated lines and was used here
	Use sort then uniq -c which shows how many times something repeats
```
9.	UsvVyFSfZZWbi6wqC7dAFyFuR6jQQUhr
```
	Strings only shows back human readable stuff
	Only one line one possible to be a password
```
10.  truKLdjsbJ5g7yyJ2X2R0o3A5hqjfuLk
```
	base64 to decode
	cat data.txt then base64 -d for decode
```
11. IFukwKGsFW8M0q3IRFqrxE1hxTNEbUPR
```
	used cat to see data was messed up just had to move letters 13 times over
	rot13 is something to install to move over 
```
12. 5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu
```
	xxd is a hexdump tool which is one this was encoded in
	xxd -reverse data.txt 
	It then makes it into unreadable
	When you look at the file its a gzip compressed
	convert the file to gz file
	These are tar files
	Final step is a ACII File 
```
13. 8ZjyCRiBWFYkneahHwxCV3b2a10RpYL
```
	no password for level 14 just have to ssh into own computer
	ssh -i sshkey.private localhost bandit14
	then type yes
```
14. 4wcYUJFw0K0XLShlDzztnTBHiqxU3b3e
```
	this was about finding the acutal pass for bandit 14
	final format was cat <password> | nc localhost 30000
```
15. BfMYroe26WYalil77FoDi9qh59eK5xNR
			
