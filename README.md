---

# Text Processing Commands README

This README file provides an overview of various text processing commands and their usage in the context of `file.txt` and `words.txt`.

## 1. grep Command

The `grep` command is a powerful tool for searching patterns within text files. The following command searches for phone numbers in the format `(###) ###-####` or `###-###-####` in `file.txt`.

This command utilizes the `-E` flag to enable extended regular expressions for complex pattern matching.

## 2. sed Command

The `sed` command is used for text stream editing. The following command prints the 10th line of `file.txt`.

The `-n` option suppresses automatic printing of pattern space, and `10p` prints the 10th line.

## 3. Bash Loop

The `for` loop in Bash iterates over words in the first line of `file.txt`, printing each word on a separate line.

This loop extracts each word from the first line and prints them individually.

## 4. Text Transformation Pipeline

The following command processes the content of `words.txt` to count and display unique words with their frequencies.

- `tr -s ' ' '\n'`: Translates spaces to newlines, ensuring each word is on its own line.
- `sort`: Sorts the words alphabetically.
- `uniq -c`: Counts the occurrences of each unique word.
- `sort -r`: Sorts the words by count in descending order.
- `awk '{ print $2, $1 }'`: Prints the word followed by its count.

Feel free to modify and expand upon these commands as needed for your specific use case. If you have any questions or need further assistance, please refer to the documentation of each command or seek help from your system administrator.
