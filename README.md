# Creating-file-in-Python
This simple program will show you how to take a user's input and then write it to a file. This was a school assignment for me.

    # Naming the file
    fileName = input('Please enter the name of the file you would like to create: ')

    # Asking user to enter all necessary information.
    userName = input('Please enter your full name: ')
    address = input('Please enter your street address: ')
    phoneNumber = input('Please enter your phone number: ')

    fileNameFinal = f'{fileName}.txt'

    # Writing and creating the file.
    with open(fileNameFinal, 'w') as contents: # Opening file
        contents.write(f'{userName}, {address}, {phoneNumber}') # Writing to file

    # Reading and printing the file contents.
    with open(fileNameFinal, 'r+') as contents:
        print(contents.read())
        contents.close()
