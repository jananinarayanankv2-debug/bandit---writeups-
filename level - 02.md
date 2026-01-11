# Bandit Level 2 → Level 3

## Level Goal
The password for the next level is stored in a file called `spaces in this filename`.

## Given Information
Username: bandit2  
Host: bandit.labs.overthewire.org  
Port: 2220  

## Approach
The file name contains spaces, so it must be accessed using quotes or escape characters.

## Commands Used
ssh bandit2@bandit.labs.overthewire.org -p 2220  
ls  
cat "spaces in this filename"

## Explanation
Linux treats spaces as separators.  
Using quotes allows us to read the full file name correctly.

## Password for Next Level
UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK

## Key Learning
How to access files with spaces in their names.
	
