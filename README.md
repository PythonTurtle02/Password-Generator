# Password-Generator
The code uses the random module in Python to generate a random password. It defines different sets of characters including lowercase letters, uppercase letters, numbers, and symbols. These sets are combined into a single string called combination. The code then selects characters randomly from combination and forms an 8-character password. 

1 - import random: This line imports the random module in Python, which provides functions to generate random numbers, sequences, and selections.
2 - lower_case = "abcdefghijklmnopqrstuvwxyz": This line defines a string variable lower_case that contains all lowercase letters of the English alphabet.
3 - upper_case = "ABCDEFGHIJKLMNOPQRSTUVWXYZ": This line defines a string variable upper_case that contains all uppercase letters of the English alphabet.
4 - numbers = "0123456789": This line defines a string variable numbers that contains all the digits from 0 to 9.
symbols = "@#$%&*?": This line defines a string variable symbols that contains a set of special characters that can be used in passwords.
5 - combination = lower_case + upper_case + numbers + symbols: This line concatenates all the previously defined string variables (lower_case, upper_case, numbers, and symbols) to create a single string called combination. This string represents the pool of characters from which the password will be generated.
6 - length_of_password = 8: This line defines an integer variable length_of_password and sets it to 8. It represents the desired length of the generated password.
7 - password = "".join(random.sample(combination, length_of_password)): This line generates the password. It uses the random.sample() function to select length_of_password number of characters randomly from the combination string. The random.sample() function ensures that each character is chosen only once. The selected characters are then joined together into a single string using the "".join() method and assigned to the password variable.
8 - print("The Generated Password is :", password): This line prints the generated password to the console, along with the message "The Generated Password is :".
This code generates a random password of length 8, comprising a combination of lowercase letters, uppercase letters, numbers, and symbols.
