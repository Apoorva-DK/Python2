# Python2
Certainly! Creating a "Word Counter" program in Python is a great way to practice basic string manipulation and programming logic. Here’s a simple Python script that counts the number of words in a given text input:

```python
def word_counter(text):
    # Remove leading and trailing whitespaces
    text = text.strip()
    
    # Split the text into words
    words = text.split()
    
    # Count the number of words
    num_words = len(words)
    
    return num_words

def main():
    print("Welcome to the Word Counter program!")
    print("Enter some text and I will count the words for you.")
    
    # Get user input
    text = input("Enter your text: ")
    
    # Count words
    num_words = word_counter(text)
    
    # Display the result
    print(f"\nNumber of words in the text: {num_words}")

if __name__ == "__main__":
    main()
```

### Explanation:

1. **word_counter function**: 
   - `strip()` method is used to remove any leading or trailing whitespaces from the input text.
   - `split()` method splits the text into a list of words based on whitespace (default behavior).
   - `len()` function counts the number of elements (words) in the `words` list.

2. **main function**:
   - Displays a welcome message and prompts the user to enter text.
   - Calls `word_counter` function with the user-provided text.
   - Prints the number of words counted.

### How to Use:

- Copy the above code into a Python environment (like IDLE or VSCode with Python extension).
- Run the script.
- Enter any text when prompted.
- The program will output the number of words in the entered text.

### Example Usage:
```
Welcome to the Word Counter program!
Enter some text and I will count the words for you.
Enter your text: Hello world! This is a simple word counter program.

Number of words in the text: 9
```

This basic program can be expanded further to handle more complex scenarios, such as counting words in a file or excluding certain types of characters from word counts.
