# Commands Used
## Level_0
ssh bandit0@bandit.labs.overthewire.org -p 2220

## Level_0 ---> Level_1
ls -alps

ls -a (--all) Do not ignore entries starting with '.'

ls -l Use a long listing format

ls -p Append / indicator to directories

ls -s Print the allocated size of each file, in blocks

cat Concatenate files and print on the standard output

## Level_1 ---> Level_2
la -alps

cat ./ To open a file of a special character. For example, "-"

## Level_2 ---> Level_3
la -alps

cat "spaces in this filename" in order to skip  cat spaces\ in\ this\ filename

## Level_3 ---> Level_4
cd Change directory

ls -alps

cat

## Level_4 ---> Level_5
ls

cd

file Determines the file type

## Level_5 ---> Level_6
find ./ -size 1033c
to find and open the file of a given size (in this case : 1033)

## Level_6 ---> Level_7
find 

du

grep








