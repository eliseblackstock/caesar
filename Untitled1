#This is a tutorial from the book Invent Your
#Own Computer Games with Python

#Caesar cipher
SYMBOLS = 'ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz' #
MAX_KEY_SIZE = len(SYMBOLS) # The key has to be of the range of 1-52
defined concept varible so is establishsing the alphabet

def getMode(): // defining a function that you are later going to call
    while True:
        print('Do you wish to encrypt or decrypt a message?')
        mode = input().lower()
        if mode in ['encrypt', 'e', 'decrypt', 'd']:
            return mode
        else:
            print('Enter either "encrypt" or "e" or "decrypt" or "d".')

def getMessage(): # if there not giving the user a key from 1-52 then the user will keep on going until they do.
    print('Enter your message: ')
    return input()

def getKey():
    key = 0
    while True:
        print('Enter the key number (1-%s)' % (MAX_KEY_SIZE))
        key = int(input())
        if (key >= 1 and key <= MAX_KEY_SIZE): if the key is less or equal to 1
            return key

def getTranslatedMessage(mode, message, key):
        key = -ke # if mode is decrypt, move the key backwards through alphabet
    translated = '' #

    for symbol in message:
        symbolIndex = SYMBOLS.find(symbol)
        if symbolIndex == -1: #Symbol not found in SYMBOLS
            #Just add this symbol without any change
            translated += symbol
        else:
            #Encrypt or decrypt
            symbolIndex += key
        if symbolIndex >= len(SYMBOLS): # this is where the shift starts happening
            symbolIndex -= len(SYMBOLS) # the symbol or character becomes the encrypted or decrypted letter using the length of the symbol and key provided.
        elif symbolIndex < 0:
            symbolIndex += len(SYMBOLS)

        translated += SYMBOLS[symbolIndex] #
    return translated # if key is geven to either 1 or 52 it will hit max size.

mode = getMode() # whether the user wnates to encrypt or decryt their message and these are the call funtions
message = getMessage() #getting the message that the user wants to decrypt or encrypt
key = getKey() # forces key given to integer format
print('Your translated text is: ')
print(getTranslatedMessage(mode, message, key)) # print statements
