# Task 
Kevin and Stuart want to play the 'The Minion Game'. You have to determine the winner of the game and their score.

## Game Rules
Both players are given the same string, s.
Both players have to make substrings using the letters of the string s.
Stuart has to make words starting with consonants.
Kevin has to make words starting with vowels.
The game ends when both players have made all possible substrings.

## Scoring
A player gets +1 point for each occurrence of the substring in the string s.

## For Example:
String s = BANANA
Kevin's vowel beginning word = ANA
Here, ANA occurs twice in BANANA. Hence, Kevin will get 2 Points.

# Code 
```python 
def minion_game(string):
    vowels = 'AEIOU'
    str_length = len(string)
    my_score, stu = 0,0

    for i in range(str_length):
        if s[i] in vowels:
            my_score += (str_length - i)
        else:
            stu += (str_length - i)


    if my_score > stu:
        print ('Kevin', my_score)
    elif stu > my_score: 
        print ('Stuart', stu)
    else:
        print ('Draw')



if __name__ == '__main__':
    s = input()
    minion_game(s)
```
