#challenge every day python
#day 1
#Random pasword generator
#Rules length of password should always be between 3 - 100 characters

import string, random

characters = string.printable
length = random.randint(3,100)
password = []

for i in range(length):
    password.append(random.choice(characters))

with open('password.txt','a') as f:
    f.write(''.join(password))
