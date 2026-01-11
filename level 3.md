# Bandit Level 3 → Level 4

## Level Goal
The password is stored in a hidden file inside the `inhere` directory.

## Given Information
Username: bandit3  
Host: bandit.labs.overthewire.org  
Port: 2220  

## Approach
Hidden files start with a dot. We must use special listing options to see them.

## Commands Used
ssh bandit3@bandit.labs.overthewire.org -p 2220  
cd inhere  
ls -a  
cat .hidden

## Explanation
`ls -a` shows hidden files.  
The `.hidden` file contains the password.

## Password for Next Level
pIwrPrtPN36QITSp3EQaw936yaFoFgAB

## Key Learning
How to view and read hidden files in Linux.
