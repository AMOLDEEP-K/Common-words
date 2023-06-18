# Common-words
## Overview
The program "common_words" is designed to analyze text files in a specified directory and provide information about the frequency of words in those files. The program offers two optional functions: finding the highest frequency rank of a specific word across the files or identifying the word that is the Nth most common across the largest number of files. The program expects a directory containing text files as a mandatory argument.

## Usage
The program can be executed using the following command format:

 **common_words [-w word | -nth N] \<directory of text files\>**


## Optional Arguments
### -w word
If the optional argument -w followed by a word is provided, the program will determine the frequency rank of that word in each text file and report the highest rank. The output will include the text file where the specified word has the highest frequency rank and the rank itself.

### -nth N
If the optional argument -nth followed by an integer N is provided, the program will identify the word that is the Nth most common across the largest number of files in the specified directory. The output will include the word and the number of files in which it is the Nth most common.

### No Options
If no options are provided, the program assumes that the user wants to find the word that is the most common across the largest number of files. In this case, the program will report the word and the number of files in which it is the most common.

## Assumptions and Considerations
The program assumes that all text files in the specified directory have the ".txt" file extension.
A word is considered as a sequence of one or more letters. Hyphenated words or word pairs should be treated as separate words.
The program preserves the letter case of the words and does not convert them to lowercase.
