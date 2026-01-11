# Bandit Level 6 → Level 7

## Level Goal
The password is stored somewhere on the server and has the following properties:
- Owned by user bandit7
- Owned by group bandit6
- 33 bytes in size

## Given Information
Username: bandit6  
Host: bandit.labs.overthewire.org  
Port: 2220  

## Approach
We search the entire system using `find` with ownership and size filters.

## Commands Used
ssh bandit6@bandit.labs.overthewire.org -p 2220  
find / -user bandit7 -group bandit6 -size 33c 2>/dev/null  
cat /var/lib/dpkg/info/bandit7.password

## Explanation
`find /` searches from the root directory.  
Ownership and size filters help find the exact file.  
Errors are hidden using `2>/dev/null`.

## Password for Next Level
HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs

## Key Learning
How to search system-wide files using ownership and size.
	
