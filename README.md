# Password-Generator

import random
import string

password_string = ""

while True:

    length = input("How many characters would you like your password to have? \n:")
    for i in range (0, int(length)):
        password_string = password_string + random.choice(string.printable)
    print(password_string)

    answer = input("Are you satisfied with this password, yes or no? ")
    if answer.lower() in 'yes':
        break
