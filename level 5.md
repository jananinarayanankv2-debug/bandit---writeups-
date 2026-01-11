# Bandit Level 5 → Level 6

## Level Goal
The password is stored in a file somewhere under the `inhere` directory and has the following properties:
- Human-readable
- 1033 bytes in size
- Not executable

## Given Information
Username: bandit5  
Host: bandit.labs.overthewire.org  
Port: 2220  

## Approach
We must search for a file that matches all the given conditions.  
The `find` command is used to filter files by size, type, and permissions.

## Commands Used
ssh bandit5@bandit.labs.overthewire.org -p 2220  
cd inhere  
find . -type f -size 1033c ! -executable  
cat ./maybehere07/.file2

## Explanation
`find` searches all files under `inhere`.  
`-size 1033c` finds files of exactly 1033 bytes.  
`! -executable` filters out executable files.  
The matching file contains the password.

## Password for Next Level
DXjZPULLxYr17uwoI01bNLQbtFemEgo7

## Key Learning
How to use `find` with filters like size and permissions.

