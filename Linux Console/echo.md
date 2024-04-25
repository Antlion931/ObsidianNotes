#book 

[[echo]] displays a text. It is not very useful in it own, however it it very needed for more complex behaviours.

## Examples
> [[echo]] "Hello, World!" | [[less]]

With [[echo]] and [[pipe]] we can send some text to commends that read input.

>[[echo]] -n -e "Here\\b\\c\\t\\a\\n\\here" > test.txt

- `-n` Don't print new line at the end
- `-e` enable special characters with backslash

It lets you create a file with a specific characters.