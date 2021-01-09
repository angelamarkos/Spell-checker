# Spell-checker
We will create spell-checker step by step.

Step 1. Writing utils for spell checker

1. In one file utils.py create function that will count two strings Levenshtein distance.

The Levenshtein distance between two strings a, b (of length |a| and |b| respectively) is given by leva,b(|a|,|b|) where:
![alt text](https://23o0161033pm1289qo1hzrwi-wpengine.netdna-ssl.com/wp-content/uploads/2017/01/Maths-768x162.jpg)

where 1(ai≠bi) is the indicator function equal to 0 when ai≠bi and equal to 1 otherwise, and leva, b(i,j) is the distance between the first i characters of a and the first j characters of b.

2. Create function in utils.py which calculate Soundex code for string:

Algorithm steps for Soundex code are:

Copy the first character of the input string to the first character of the output string

For subsequent characters in the input string, add digits to the output string according to the table below, up to a maximum of three digits (ie. a total output string length of 4). Note that a number of input letters are ignored, including all vowels. Also, further occurences of an input letter with the same encoding are ignored.

If we reach the end of the input string before the output string reaches 4 characters, pad it to the right with zeros.

----Encoding Table----

Input letter	 Encoding
A	------------ 0
B	------------ 1
C	------------ 2
D	------------ 3
E	------------ 0
F	------------ 1
G	------------ 2
H	------------ 0
I	------------ 0
J	------------ 2
K	------------ 2
L	------------ 4
M	------------ 5
N	------------ 5
O	------------ 0
P	------------ 1
Q	------------ 2
R	------------ 6
S	------------ 2
T	------------ 3
U	------------ 0
V	------------ 1
W	------------ 0
X	------------ 2
Y	------------ 0
Z	------------ 2

3. create main.py and use functions from utils.py

When you run your code this will be printed:
Exp1: Chose option:
        1. Levenshtein
        2. Soundex
       Type 1 or 2: 1
       First string: kitten
       Seccond string: sitting
       Levenshtein distance for "kitten" and "sitting" is 3
Exp2: Chose option:
        1. Levenshtein
        2. Soundex
       Type 1 or 2: 2
       Input string: example
       Soundex code for "example" is E251
       
Step 2. TBD.
