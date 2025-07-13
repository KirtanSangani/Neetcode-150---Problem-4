# Neetcode-150---Problem-4

7/13/2025

## Thought Process
At the beginning, I was a little confused as to how to count each letter for both strings. I was thinking of either doing a hash table or a dictionary so I could have values corresponding to each letter. I would try a dictionary but found it time consuming trying to count each value for two dictionaries. Additionally, it would have taken up more memory space than necessary. 

## Solution
I decided to go with two Lists instead. I initialized both Lists to contain 26 spaces, one for each letter. I would then go through each letter of both strings and "mark" their corresponding spot in each List. It took me a while to find out how to mark the correct spot, but figured it out using the ord() function. This function allows me to find the ASCII value of each letter, and since all letters will always be lowercase, by subtracting the ASCII value of the letter by the ASCII value of 'a', I can find the index that corresponds to that letter. After the for loop runs through, I would check to see if both Lists are the same, if they are, return true, if not, return false.  

Final Solution - 20 ms

Complexity - O(n)

## Takeaways
I learned how to find the index of the alphabet (a - 1, b - 2, c - 3, etc.) I also am starting to figure out how to properly manage space and memory for things like Lists vs Hash Tables vs Dictionaries. 