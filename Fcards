import os, random
import string

while True:
    name = raw_input("Your Name: ").capitalize() # ask inside the loop
    if name and name.isalpha():
        print "Hi %s " %name
        break # leave the loop if done
    elif name and name.isdigit():
        print "Name must be Alphabet characters only!"
    else:
        print "Please enter something valid."

F1 = open('words.txt', 'r')
F2 = open('meaning.txt', 'r')
F1c = F1.readlines()
F2c = F2.readlines()

count = 0
score = 0

while count < 15:
	os.system('clear')
	wordnum = random.randint(0, len(F1c)-1)
	print 'What is:  ', F1c[wordnum], ''
	options = [random.randint(0, len(F2c)-1),random.randint(0, len(F2c)-1),random.randint(0, len(F2c)-1),random.randint(0, len(F2c)-1),random.randint(0, len(F2c)-1),]
        options[random.randint(0, 3)] = wordnum
        
        print '1 -', F2c[options[0]],;print '2 -', F2c[options[1]],;print '3 -', F2c[options[2]],;print '4 -', F2c[options[3]],
        answer = int(raw_input('\nYou  choose number ?: '))
        if options[answer-1] == wordnum:
            raw_input('\nCorrect! Hit enter...')
            score = score + 1
        elif options[answer-1] not in range(wordnum):
            print ("Out of range...")
        else:
            raw_input('\nWrong! Hit enter...')
            count = count + 1
            print '\nYour score is:', score

