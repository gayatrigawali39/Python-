# Python-
import random
import string

def generate_password(length=8):
    chars = string.ascii_letters + string.digits + string.punctuation
    return ''.join(random.choice(chars) for _ in range(length))

if __name__ == "__main__":
    length = int(input("Enter password length: "))
    print("Your Password:", generate_password(length))
