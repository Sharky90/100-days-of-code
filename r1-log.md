# #100DaysOfCode Log - Round 1 - [Emin Avdovic]

The log of my #100DaysOfCode challenge. Started on [September 05, Thursday, 2019].

## Log

### R1D1 
//Day 1:September 05. Thursday//
Today's Progress: I have learned about "Operators and Branching" (code structure, python boolean types and their order of operation) through MIT course Intro to CS and programming with Python.

//Day 2:September 06. Friday//
Today's Progress: Just did the 'Bindings' and 'Strings' chapter and learned how to manipulate different operations in a string.
Special thanks to MIT's intro to cs and programming with python for in detail explanation.  

//Day 3:September 07. Saturday//
Today's Progress: Learned how to control loops ( for loops & while loops) and how to break statements.

//Day 4:September 08. Sunday//
 Learned about 'Iterations' and crunched some codes using 'while' loops and 'for' loops
 
//Day 5:September 10. Tuesday//
Was coding yesterday but forgot to post...won't happen again...lol anyway I went through 'Iteration' and ' 'guess and check chapter' where I was finding a cube root of an integer. 

//Day 6:September 11. Wednesday//
Wow how many version are there with the same output?! This was a case instead of nesting a for loop inside a while loop, I had to nest a while loop inside a for loop to get same results... 

//Day 7:September 12. Thursday//
Today I've learned about 'approximate solutions' (starting with a guess and increment by some small value for some small epsilon)... The exercises are getting harder I must crunch more codes and tackle this course! 💻🤓

//Day 8:September 13. Friday//
Ok... The left problem was the 'AHAa' moment and I was very very happy that I solved it but the right problem I've spent hours... It is supposed to be 2 ... or ?!  
Right Exercise:
s = "azcbobobegghakl"
word = "bob"
count = s.count(word)
for word in s:
      if word == 'bob':
         count += 1
print("Number of times bob occurs is: " + str(count))
Number of times bob occurs is: 1

Left Exercise:
count = 0 
s = "azcbobobegghakl"
for letter in s:
        if letter == 'a' or letter == 'e' or letter == 'i' or letter == 'o' or letter == 'u':
                for s in range(1):
                        count += 1
print("Number of vowels: " + str(count))
Number of vowels: 5    

//Day9: September 14.Saturday//
Ok today i learned about 'approximate solutions','bisection search'... From tomorrow I am gonna continue with "Automate The Boring Stuff With Python" by Al Sweigart. 
I want to try and make some fun mini projects... 

//Day 10: September 15.Sunday//
Spent time with family but still managed to read about 'Functions' and wrote this funny exercise 'magic8ball' in python... I have to learn one more chaprer 'Lists' and then I'll be able to begin writing some fun programs...😁💻🤗

import random

def getAnswer(answerNumber):
      if answerNumber == 1:
            return 'It is certain'
      elif answerNumber == 2:
            return 'It is decidedly so'
      elif answerNumber == 3:
            return 'Yes'
      elif answerNumber == 4:
            return 'Reply hazy try again'
      elif answerNumber == 5:
            return 'Ask again later'
      elif answerNumber == 6:
            return 'Concentrate and ask again'
      elif answerNumber == 7:
            return 'My reply is no'
      elif answerNumber == 8:
            return 'Outlook not so good'
      elif answerNumber == 9:
            return 'Very doubtful'

r = random.randint(1, 9)
fortune = getAnswer(r)
print(fortune)

//Day 11: September 16.Monday//
Today I learned about 'Local and Global Scope' and when their variables can be used and how... but then... hahahahaha this program cracked me up 🤣🤣🤣
# This is a guess the number game.
import random
secretNumber = random.randint(1, 20)
print('I am thinking of a number between 1 and 20.')

# Aske the player to guess 6 times
for guessesTaken in range(1, 7):
      print('Take a guess.')
      guess = int(input())

      if guess < secretNumber:
            print('Your guess is too low.')
      elif guess > secretNumber:
            print('Your guess is too high.')
      else:
            break             # This condition is the correct guess!

if guess == secretNumber:
      print('Good job! You guessed my number in ' + str(guessesTaken) + ' guesses!')
else:
      print('Nope. The number I was thinking of was ' + str(secretNumber))
      
//Day 12: September 17.Tuesday//
Busy day but still managed to setup Visual Studio Code while watching Traversy Media adding 15 extensions... Will code tomorrow and go through 'Lists' chapter for python...
Good Night...😴💤🛌

//Day 13: September 17.Wednesday//
Spent a couple of hours on this 'Collaz' problem I was really into it... I will not skip this problem... but now I am... tired... gonna sleep... dream about the solution... its there somewhere... out there... deep space.. INTERSTELLAR... 🤣🛌💤🛰️🚀🌘☄️

                                #Function definition 
def collatz(number):
   if number == 2:
      return(number // 2)
   elif number == 1:
      return(3 * number + 1)
                                               
                                               
                               #Ask for input integer
print('Enter number: ')
number = int(input())

//Day 14: September 18.Thursday//
Finally after a lot of trial and error... solved it... although i think I will have to read more about algorithms and problem solving tips... Can anyone recommend me a book?

                                                   #Function definition 
def collatz(number):
   if number % 2 == 0:
      return number // 2
   else:
      return 3*number + 1
      return result
                                                   #Ask for input integer
try:
   n = int(input("Enter number: "))
   while n != 1:
      print(n)
      n = collatz(abs(n))
   if n == 1:
      print(n)
except ValueError:
   print('Error: Try again.')
      

### R1D2
