def isWhiteSpace(character):
    return character == " " or character == "\n" #detects for whitespace and if rolls to a new line

def slice(sentence): #this is a function that to divides a sentence into words
    words = [] #This is an empty list
    begginingOfWord = 0
    currentCharacter = 0
    for character in sentence:   #This will take us through the chacters in the sentence
        if isWhiteSpace(character):
            word = sentence[begginingOfWord:currentCharacter]  #This slices the found letters from the list
            words.append(word.lower()) #This adds and lowercases what we "sliced" from the sentence to the empty list
            begginingOfWord = currentCharacter + 1  #This is a counter that increases allows you to start at the next word by counting the currentCharacter
                                                    # index plus the whitespace
        #    currentCharacter += 1                  These next 2 lines were removed because it is redundant
        #else:
        currentCharacter += 1 # skips past the whitespace to the start of the next word
    return words
def countWords(sentence):
    wordCount = {}
    words = slice(sentence)
    for word in words:
        if word in wordCount:
            wordCount[word] += 1

    else:
        wordCount[word] = 1
    print wordCount



countWords("hello this is my sentence this is a sentence")
