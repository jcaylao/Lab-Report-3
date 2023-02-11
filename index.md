# **Lab Report 3 - Researching Commands**

## **The `grep` command**

### **`grep -r`**

The `-r` stands for recursive, in which this command will run to recursively search through all the files in the directory you are currently in. Given a string to search for, it will print the section of the file that contains the word and highlights it. This is useful to search through all the files within the given directory including the folders within it, rather than having to cd into each folder to search through each file.

Example 1:

![Image](https://github.com/jcaylao/Lab-Report-3/blob/main/Screenshot%202023-02-10%20152629.png?raw=true)

Example 2:

![Image](https://github.com/jcaylao/Lab-Report-3/blob/main/Screenshot%202023-02-10%20152920.png?raw=true)

I will be using the `-r` option in the upcoming examples.

### **`grep -i`**

The `-i` option of grep is used to ignore uppercases or lowercases, meaning as long as the words match, it would not matter whether it was uppercase or lowercase. This is useful because if this option were not used with a word that was inputted with all uppercase, then the matches would not show up because the computer would not be able to detect the match. Through these examples, you can see that the files do not show up unless the `-i` option is used due to the cases not matching up with eachother.

Example 1:

![Image](https://github.com/jcaylao/Lab-Report-3/blob/main/Screenshot%202023-02-10%20153900.png?raw=true)

Example 2:

![Image](https://github.com/jcaylao/Lab-Report-3/blob/main/Screenshot%202023-02-10%20154017.png?raw=true)

### **`grep -w`**

The -w option is used to search for text that matches the inputted word exactly. This would be useful in narrowing down the search because some text may show up but may not match the given up due to the word containing the input within the string, as shown in example 1. This may also occur with plural words or verbs in which they have suffixes at the end, as shown in example 2.

Example 1: 

input `grep "run"`

![Image](https://github.com/jcaylao/Lab-Report-3/blob/main/Screenshot%202023-02-10%20160559.png?raw=true)

input `grep -w "run"`

![Image](https://github.com/jcaylao/Lab-Report-3/blob/main/Screenshot%202023-02-10%20160622.png?raw=true)

Example 2: 

input `grep "study"`

![Image](https://github.com/jcaylao/Lab-Report-3/blob/main/Screenshot%202023-02-10%20160846.png?raw=true)

input `grep -w "study"`

![Image](https://github.com/jcaylao/Lab-Report-3/blob/main/Screenshot%202023-02-10%20161024.png?raw=true)

### **`grep -l`**

The option `-l` (lowercase L) is used to return the filenames only, rather than returning a whole section of text that contains the inputted string. This would be useful in cases  where there is a large amount of files and long sections of texts when the terminal would not be able to hold all of the information and cuts off some of it due to running out of space on the terminal (cannot scroll up any further).

Example 1: 

![Image](https://github.com/jcaylao/Lab-Report-3/blob/main/Screenshot%202023-02-10%20162206.png?raw=true)

Example 2:

![Image](https://github.com/jcaylao/Lab-Report-3/blob/main/Screenshot%202023-02-10%20162141.png?raw=true)

## **Sources**
https://www.geeksforgeeks.org/grep-command-in-unixlinux/
https://alvinalexander.com/linux-unix/recursive-grep-r-searching-egrep-find/
