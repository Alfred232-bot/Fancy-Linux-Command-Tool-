#!/bin/bash

# Fancy Linux Command
# Combine grep and head
# Searches for a word in a file and display the first matching lines

if [ $# -ne 3 ]; them
    echo "Usage: ./fancy.sh <file> <number>" 
    exit 1
fi

WORD=$1
FILE=$2
NUMBER=$3

if [ ! -f "$FILE" ]; then
    echo "Error: '$FILE' dose not exist."
    exit 1
fi

echo "Searching for '$WORD' in $FILE..."
echo "Showing the first $NUMBER results:"
echo "---------------------------------"

grep "$WORD" "$FILE" | head -n "$NUMBER"







