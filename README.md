<picture align="center">
  <img alt="Pandas Logo" src="https://shbpacademy.com/wp-content/uploads/2023/01/Depositphotos_475507236_XL-840x450.jpg">
</picture>

-----------------

# Project: Secure Password Generator

| | |
| --- | --- |
| My channel | [[Rutube](https://rutube.ru/plst/909045/)] |
| My channel | [[plvideo](https://plvideo.ru/playlist?list=SuymwXRNSHg3)] |
| My github | [[GitHub](https://github.com/migolovina/)]|

## What is this?

My project on the topic "Secure Password Generator".

## Goal

Write a program that creates random passwords of a given length using letters, numbers and special characters.

# What you will need

- Language: **Python** (you can use any online compiler or installed IDE).

- Libraries: `random` (built-in, nothing else needs to be installed).

# Why this is a good project:

✅ Simple and understandable for beginners.

✅ Useful in real life.

✅ Can be expanded and complicated.

# Program code

```python
import random
import string

def generate_password(length=12):
    # Symbols that will be used to create the password
    characters = string.ascii_letters + string.digits + string.punctuation
    # Generate password
    password = ''.join(random.choice(characters) for _ in range(length))
    return password

# Main program
if __name__ == "__main__":
    print("Secure Password Generator")
    length = int(input("Enter password length: "))
    password = generate_password(length)
    print(f"Your password: {password}")

