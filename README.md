#import random

def generate_google_voice_numbers():
    numbers = []
    while True:
        number = random.randint(1000000000, 9999999999)
        if str(number).endswith('5487'):
            numbers.append(number)
            if len(numbers) == 10:
                break
    return numbers

google_voice_numbers = generate_google_voice_numbers()
print(google_voice_numbers)
