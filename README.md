# codsoft_3
import random
import string
def Pass(length):
    char=string.ascii_letters+string.digits+string.punctuation
    password = ''.join(random.choice(char) for _ in range(length))
    return password
try:
    length =int(input("enter desired length of password"))
    Pass=Pass(length)
    print("generated password:",Pass)
except ValueError:
    print("error")
