import random

def generate_captcha():
    # Define the possible characters for the Captcha
    characters = 'ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789'
    
    # Generate a Captcha of 5 characters
    captcha = ''.join(random.choice(characters) for _ in range(5))
    
    return captcha

# Testing the Captcha generator multiple times
for _ in range(5):
    print(generate_captcha())
