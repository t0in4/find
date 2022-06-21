# find

## find multiple files and copy them into folder

### $ find . -type f \( -name "*smth.jpg" -o -name "*onemore.jpeg" -o -name "*sometype" \) -exec cp "{}" /path/to/folder \;
