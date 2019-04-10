# Lists Section Goals
- [Append user input to a list using a loop](#append-in-loop)
- [Count the number of words that start/end with a specific string](#count-startswith)
- Find the largest item in a list
- Items whose length is greater than a specific value.
- Find words that have more than a specific number of vowels.
- Find words with the largest consonant streak.
- Filter a list (create a new list) of words to include only words that begin with a vowel.

## Append in loop
```python
# create a loop that will read in 5 integer values into a list.

numbers = []  # initialize list
for pos in range(5):
    num = int(input(f"Enter a number ({pos+1} of 5): "))
    numbers.append(num)  # append number to list

print(numbers)
```

## Count Startswith
```python
# create a program that will count the number of words that start with 
# the letter "h"

words = ["hello", "hat", "bat", "shell", "tv", "livingroom", "heavy"]
count = 0
for word in words:
    if word.startswith("h"):  # modify to check first two letters
        count += 1

print(count)