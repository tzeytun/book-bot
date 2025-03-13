# Book Bot

Book Bot is a simple Python application that analyzes a book text file and provides a report on the word count and character frequency.

## Features

- Count the total number of words in a book.
- Count the frequency of each character in the book.
- Generate a sorted list of characters based on their frequency.
- Display a report containing the word count and character frequency.

## Requirements

- Python 3.x

## Installation

Clone the repository:
    ```bash
    git clone https://github.com/tzeytun/book-bot.git
    cd book-bot
    ```


## Usage

Run the `main.py` script with the path to the book text file as an argument:
```bash
python3 main.py <path_to_book>
```

Example:
```bash
python3 main.py books/frankenstein.txt
```

## Files

- `main.py`: The main script that handles input, processes the book text, and generates the report.
- `stats.py`: Contains helper functions for counting words, counting each character, and sorting the character count.

## Functions

### main.py

- `get_book_text(path)`: Reads the content of the book from the given path.
- `main()`: The main function that parses the command-line arguments, processes the book text, and prints the report.
- `print_report(book_path, num_words, chars_sorted_list)`: Prints the analysis report.

### stats.py

- `count_words(book_text)`: Returns the total number of words in the book text.
- `each_character(book_text)`: Returns a dictionary with the frequency of each character in the book text.
- `sort_on(d)`: Helper function for sorting based on character frequency.
- `chars_dict_to_sorted_list(num_chars_dict)`: Converts the character frequency dictionary into a sorted list of characters.

## Example Output

```
============ BOOKBOT ============
Analyzing book found at books/my_favorite_book.txt...
----------- Word Count ----------
Found 12345 total words
--------- Character Count -------
a: 678
b: 123
c: 234
...
============= END ===============
```

## Attribution

I would like to express my gratitude to [Boot.dev](https://boot.dev) for helping me with this project.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.