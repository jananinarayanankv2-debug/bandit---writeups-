# Bandit Level 1 → Level 2

## Level Goal
The password for the next level is stored in a file called `-` located in the home directory.

## Given Information
Username: bandit1  
Host: bandit.labs.overthewire.org  
Port: 2220  

## Approach
The file name starts with a dash, so it must be accessed using a special method.

## Commands Used
ssh bandit1@bandit.labs.overthewire.org -p 2220  
ls  
cat ./-

## Explanation
Files that start with `-` are treated as options by commands.  
Using `./-` tells Linux that it is a file in the current directory.

## Password for Next Level
CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9

## Key Learning
How to read files with special characters in their names.
