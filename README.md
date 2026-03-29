## EX1 : List Operations in Python: Sum of List Items

## Aim

To write a Python program that calculates the sum of all elements in a list.

## Algorithm

1. Define a list of numbers.
2. Use Python’s built-in sum() function to calculate the total.
3. Print the result.
   
## Program
```
items=[153,147,124,102]
print(sum(items))
```

## Output

<img width="559" height="111" alt="Screenshot 2026-03-29 180800" src="https://github.com/user-attachments/assets/7adf4c9e-a113-4fc0-a9cf-ef5dc2251cbb" />

## Result

Thus, The output is successfully verified.


## Ex2 : Regex in Python: Filter Words Without the Letter 'e'

## Aim

To write a Python program that filters out and returns all elements from a list that do not contain the letter 'e', using regular expressions (regex).

## Algorithm

1. Import the re module.
2. Initialize an empty list l1 to store results.
3. Define a list of words:
      items = ['goal', 'new', 'user', 'sit', 'eat', 'dinner']
4. Iterate through each word in the list:
      Use re.search(r"e", i) to check if the word contains 'e'.
      If not, append the word to l1.
5. Print the final filtered list.
   
## Program
```
import re
words = ['apple', 'banana', 'cherry', 'date', 'fig', 'grape']
pattern = re.compile(r'^[^e]*$')
filtered_words = [word for word in words if pattern.match(word)]
print("Words without the letter 'e':", filtered_words)
```
## Output

<img width="568" height="42" alt="Screenshot 2026-03-29 181557" src="https://github.com/user-attachments/assets/af5a52d0-9df5-4da3-ab5f-12bf4b7ad441" />

## Result

The program successfully filters and returns all elements from the list that do not contain 'e',using regex


## Ex3 : Strings-Remove Nth Index Character from a String

## Aim

To write a Python program that accepts a string and removes the character at a specified index.

## Algorithm

1. Define a function named remove that takes the input string as an argument.
2. Read the index n from the user input.
3. Initialize an empty string a to store the new string.
4. Iterate over each index of the string using a for loop.
5. Check if the current index i is not equal to n.
6. If i != n, append the character at index i to string a.
7. After the loop, return the modified string a.
8. Print the final result.
   
## Program
```
def remove(string, n):
    a = "" 
    for i in range(len(string)):
        if i != n: 
            a = a + string[i]
    return a
string = input("Enter a string: ")
n = int(input("Enter the index to remove: "))
print("Modified string:", remove(string, n))
```
## Output

<img width="565" height="64" alt="Screenshot 2026-03-29 181908" src="https://github.com/user-attachments/assets/b8838c98-c887-4e0a-a7d0-81cc8fb5afbf" />

## Result

The program successfully takes a string and an index number from the user, removes the character at the specified index, and prints the modified string without that character.


## Ex4 : Strings-Palindrome Check in Python (Without Built-in Functions)

## Aim

To write a Python program to check whether the string "google" is a palindrome or not, without using built-in palindrome checking functions.

## Algorithm

1. Assign the string "google" to a variable.
2. Reverse the string manually using slicing ([::-1]).
3. Compare the original string with the reversed string.
       If they are equal, print that the string is a palindrome.
       Otherwise, print that it is not a palindrome.
4. Execute the program.
   
## Program
```
def is_palindrome(s):
    s = s.lower()
    left, right = 0, len(s) - 1
    while left < right:
        if s[left] != s[right]:
            return False
        left += 1
        right -= 1
    
    return True
```
## Output

<img width="562" height="41" alt="Screenshot 2026-03-29 182120" src="https://github.com/user-attachments/assets/e722ce0e-3256-4ac9-ac31-e88ec80a3c8d" />

## Result

The program successfully checks whether the string 'google' is a palindrome or not.


## Ex5 : Tuple in Python: Check Element Existence

## Aim

To write a Python program that checks if the element 'n' and the element 8 exist within a given tuple.

## Algorithm

1. Define a tuple x with some letters and numbers.
2. Use the in operator to check if the string 'n' exists within the tuple.
3. Use the in operator to check if the integer 8 exists within the tuple.
4. Print the results.
   
## Program
```
x = ('a', 'n', 'g', 'e', 'l', 8, 9, 3)
print('n' in x)
print(8 in x)
```
## Output

<img width="347" height="86" alt="Screenshot 2026-03-29 182356" src="https://github.com/user-attachments/assets/13a3a2e5-2583-4174-8ec0-173edf87e343" />

## Result

The program successfully checks for the existence of both the character 'n' and the number 8 in the given tuple and prints True for each, confirming their presence.
executed successfully.
