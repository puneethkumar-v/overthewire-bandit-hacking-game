# Overthewire Bandit Hacking Game:

A begginer level hacking game to imporve hacking skills

Official Website:
[overthewire.org](https://overthewire.org/wargames/)

## Format to ssh aroung different games using ssh:

```sh
ssh banditX@bandit.labs.overthewire.org -p 2220 
```

X represents the level i.e 0 - 34

Level 0's Password: bandit0
## Level 0:

Pass was hidden in the home directory's readme file:

```sh
cat readme
```
Level 1 Password: NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL

## Level 1:

Dashed files (-):

```sh
cat ./-
```
Level 2 Password: rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi

##  Level 2:

space in the middle file:

```sh
cat ./spaces\ in\ this\ filename
```
Level 3 Password: aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG 

## Level 3:

hidden file which starts with (.):

```sh
cd inhere
cat ./.hidden
```
Level 4 Password: 2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe

## Level 4:

file which start with -file0X, x in which 0 - 7 whose content can be unreadable:

```sh
cd inhere
cat ./-file07
```
Level 5 Password: lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR

## Level 5:

The password for the next level is stored in a file somewhere under the inhere directory and has all of the following properties:

human-readable
1033 bytes in size
not executable

```sh
cd ~/inhere/maybehere07
ls -al

total 56
drwxr-x---  2 root bandit5 4096 Apr 23 18:04 .
drwxr-x--- 22 root bandit5 4096 Apr 23 18:04 ..
-rwxr-x---  1 root bandit5 3663 Apr 23 18:04 -file1
-rwxr-x---  1 root bandit5 3065 Apr 23 18:04 .file1
-rw-r-----  1 root bandit5 2488 Apr 23 18:04 -file2
-rw-r-----  1 root bandit5 1033 Apr 23 18:04 .file2
-rwxr-x---  1 root bandit5 3362 Apr 23 18:04 -file3
-rwxr-x---  1 root bandit5 1997 Apr 23 18:04 .file3
-rwxr-x---  1 root bandit5 4130 Apr 23 18:04 spaces file1
-rw-r-----  1 root bandit5 9064 Apr 23 18:04 spaces file2
-rwxr-x---  1 root bandit5 1022 Apr 23 18:04 spaces file3

cat .file2
```
Level 6 Password: P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU

