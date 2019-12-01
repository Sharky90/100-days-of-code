# #100DaysOfCode Log - Round 1 - [Emin Avdovic]

The log of my #100DaysOfCode challenge. Started on [September 05, Thursday, 2019].

## Log

### R1 
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

//Day 13: September 18.Wednesday//
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

//Day 14: September 19.Thursday//
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
   
//Day 15: September 20.Friday //
So today I was reading about 'Lists' and found a cool program that goes like this... 

catNames = []
while True:
   print('Enter the name of cat ' + str(len(catNames) + 1) +
      ' (Or enter nothing to stop.):')
   name = input()
   if name == '':
         break
   catNames = catNames + [name] # list concatenation
print('The cat names are:')
for name in catNames:
   print(' ' + name)
   
//Day 16: September 21.Saturday //
Was reading about and working with 'lists' and using for loops... Just did this neat program... Taking a bit slow step by step just to understand clearly...
>>> supplies = ['pens', 'staplers', 'flame-throwers', 'binders']
>>> for i in range(len(supplies)):
	print('Index ' + str(i) + ' in supplies is: ' + supplies[i])
Index 0 in supplies is: pens
Index 1 in supplies is: staplers
Index 2 in supplies is: flame-throwers
Index 3 in supplies is: binders

//Day 17: September 22.Sunday //
Learned about 'Augmented Assignment Operators and Methods' in python'. Gonna crunch codes tomorrow at 'hakerrank' just to refresh my memory...🤓💪💻

//Day 18: September 30.Monday //  
Hey folks, yeah its been 7 days since i posted my coding progress the reason is because I had to travel for state competition in 10m air pistol. Now that I am back I've re-read some previous chapters about 'Methods' and 'Augmented operators . 

import random

messages = [
    "It is certain",
    "It is decidedly so",
    "Yes definately",
    "Reply hazy try again",
    "Ask again later",
    "Concentrate and ask again",
    "My reply is no",
    "Outlook not so good",
    "Very doubtful",
]
print(messages[random.randint(0, len(messages) - 1)])

//Day 19 October 01.Tuesday //
So today I was practicing what I learned till now through 'Finxter' and 'Codewars'  and I must say I need to improve more and fix my study habits to solve problems constantly.     

//Day 20 October 02.Wednesday//
Got a fever...very sick... tried 'CodeWars' just to practice a little... can't wait t gett well and learn new stuff from "Automate The Boring Stuff With Python".... 
🛌😷 #100DaysOfCode 

//Day 21 October 03.Thursday//

Ok folks... I must admit... After reading about 'References','copy() and deepcopy() functions, I took a practice project called 'Comma Code'... So far I'm like Sherlock finding clues and trying to solve the riddle but I am taking too much time. Is this a problem?

#Comma Code

spam = ['apples', 'bananas', 'tofu', 'cats']
spam.insert(3,  'and')
def incrementor (spam):
      return spam

print(spam)




# += this operator can do string and list concatenation
# sep = ',' separate list items with a comma
# sep = ' ' separate list items with a space
# spam.insert(3, 'and')
# def incrementor (x):
#     return   x + 1
# incrementor(4)
# returns   5

// Day 22 October 04.Friday //

Busy day... got late home...tried to solve the 'Comma Code' project... still no good... need to sleep it over and start fresh in the morning... I MUST GET IT DONE !

// Day 23 october 07.Monday //

After some time struggling with the 'Comma Code' I had to turn it down for some other time and move on with 'Dictionaries and Structuring Data'... Did this 'totalBought' project...One more chapter to go...

allGuests = {'Alice': {'apples': 5, 'pretzels': 12},
                     'Bob': {'ham sandwiches': 3, 'apples': 2},
                     'Carol': {'cups': 3, 'apple pies': 1}}

def totalBrought(guests, item):
      numBrought = 0
      for k, v in guests.items():
         numBrought = numBrought + v.get(item, 0)
      return numBrought

print('Number of things being brought:')
print('  - Apples                   ' + str(totalBrought(allGuests, 'apples')))
print('  - Cups                      ' + str(totalBrought(allGuests, 'cups')))
print('  - Cakes                    ' + str(totalBrought(allGuests, 'cakes')))
print('  - Ham Sandwiches  ' + str(totalBrought(allGuests, 'ham sandwiches')))
print('  - Apples Pies           ' + str(totalBrought(allGuests, 'apples pies')))


Number of things being brought:
  - Apples                   7
  - Cups                      3
  - Cakes                    0
  - Ham Sandwiches  3
  - Apples Pies           0
  


// Day 24 October 08.Tuesday // 
Nearly finished 'Manipulating Strings' chapter just need to do a couple of exercises and that will be it with this book... 
I will need to focus and work from now on building my own project... Oh and this code is from the last chapter...
 
def printPicnic(itemsDict, leftWidth, rightWidth):
   print('PICNIC ITEMS'.center(leftWidth + rightWidth, '-'))
   for k, v in itemsDict.items():
      print(k.ljust(leftWidth, '.') + str(v).rjust(rightWidth))

picnicItems = {'sandwiches': 4, 'apples': 12, 'cups': 4, 'cookies': 8000}
printPicnic(picnicItems, 12, 5)
printPicnic(picnicItems, 20, 6)

---PICNIC ITEMS--
sandwiches..    4
apples......   12
cups........    4
cookies..... 8000
-------PICNIC ITEMS-------
sandwiches..........     4
apples..............    12
cups................     4
cookies.............  8000
>>> 

// Day 25 October 14.Monday //
I have a template of my website which I did last year using Photoshop + Axure RP for rapid prototyping, wire-framing. So now I am learning the basics of HTML. I will go through Front-End and Back-End to make it. Also I did the lvl one HTML assessment. 🥳
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta http-equiv="X-UA-Compatible" content="ie=edge" />
    <title>Welcome to my Website!</title>
  </head>
  <body>
    <h1>Welcome to my Website!</h1>
    <p>I'm excited to eventually learn Django!</p>
    <a href="https://www.djangoproject.com/"
      >Here is a link to the official Django Website</a
    >
    <p>Here is a picture of the Python Logo:</p>
    <img
      src="https://www.python.org/static/community_logos/python-logo-master-v3-TM.png"
      alt=""
    />
    <p>Here are three reasons Django is cool</p>
    <ol>
      <li>Ridiculously Fast</li>
      <li>Reassuringly Secure</li>
      <li>Exceedingly Scalable</li>
    </ol>
    <h2>Bonus: Optional Extra Credit</h2>
    <p>Can you figure out how to make a picture a link?</p>

    <a href="https://www.djangoproject.com/"
      ><img
        src="https://www.edgica.com/wp-content/files/django-logo-big.jpg"
        alt=""
    /></a>
  </body>
</html>


// Day 26 October 16. Wednesday//
It's going pretty good with HTML, today I learned about 'Forms,Tables,Selection'... Here's what I made with it.
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta http-equiv="X-UA-Compatible" content="ie=edge" />
    <title>Hotel Feedback</title>
  </head>
  <body>
    <h1>Hotel Feedback Form</h1>
    <form method="get">
      <h2>Are you from inside the US? Or outside the US?</h2>
      <label for="inusa">Inside:</label>
      <input id="inusa" type="radio" name="loc" value="inside" />
      <label for="outusa">Outside:</label>
      <input id="outusa" type="radio" name="loc" value="outside" />
      <h2>How was your service?</h2>
      <select name="stars">
        <option value="Great">3</option>
        <option value="Okay">2</option>
        <option value="Bad">1</option>
      </select>
      <h2>Any other feedback?</h2>
      <textarea name="" id="" cols="30" rows="10"></textarea>>
      <input type="submit" name="" value="SUBMIT" />
    </form>
  </body>
</html>

// Day 27 October 17. Thursday//
So today I did an assessment of HTML lvl2. Tomorrow will be going through the fundamentals of CSS. Today was an awesome day... 😆🤗💻
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta http-equiv="X-UA-Compatible" content="ie=edge" />
    <title>Assignment Test HTML LEVEL 2</title>
  </head>
  <body>
    <h1>Course Sign Up Page</h1>
    <p>Please Note: First Name, Last Name, Password, and Email are required</p>
    <form action="THANK YOU!.html" method="GET">
      <label for="First Name">First Name:</label>
      <input
        id="First Name"
        type="text"
        name=""
        placeholder="First Name"
        required
      />

      <label for="Last Name">Last Name:</label>
      <input
        id="Last Name"
        type="text"
        name=""
        placeholder="Last Name"
        required
      />

      <p></p>

      <label for="Email">Email:</label>
      <input
        id="Email"
        type="text"
        name=""
        placeholder="name@email.com"
        required
      />
      <label for="Password">Password:</label>
      <input
        id="Password"
        type="password"
        name="Password"
        placeholder=""
        required
      />

      <p>Are you over the age of 18?</p>

      <label for="Yes">Yes:</label>
      <input type="radio" name="loc" value="Yes" />
      <label for="No">No:</label>
      <input type="radio" name="loc" value="No" />
      <p>Do you have a Credit Card or PayPal?</p>
      <select name="stars">
        <option value="Credit Card">Credit Card</option>
        <option value="PayPal">PayPal</option></select
      >
      <p></p>
      <input type="submit" name="" value="Submit Feedback" />
    </form>
  </body>
</html>

// Day 28 October 18. Friday//

Keeping up with the work... Today I was going through the basics of CSS customizing the background & border style of an html. 
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta http-equiv="X-UA-Compatible" content="ie=edge" />
    <title>CSS BASICS</title>
    <link rel="stylesheet" href="Part_2master.css" />
  </head>
  <body>
    <p>This is a paragraph, outside any div.</p>
    <div>
      <p>I'm inside the div.</p>
      <p>I'm also inside the div.</p>
      <p>Inside div <span>INSIDE SPAN!</span></p>
    </div>
  </body>
</html>

body {
  background: url(https://img2.10bestmedia.com/Images/Photos/352450/GettyImages-913753556_54_990x660.jpg);
  background-repeat: no-repeat;
}

div {
  background-color: blue;
  border-color: orange;
  border-width: 5px;
  border-style: double;
}
p {
  color: yellow;
}

span {
  background: red;
  color: black;
}

// Day 29 October 19. Saturday //

Saturday = Busyday... Managed to go through CSS(selectors ids, classes and "specificity") also finished the first CSS assessment with some minor issues... took a break... went back to it until the solutions appeared... NEVER SETTLE...🤓💻 #100DaysOfCode 
/*Welcome to your CSS Level One Assessment Test!

For this test, edit the CSS file and complete the commented tasks below!
You won't be editing and html, but the css file is linked to the html file.
Watch the video lecture for more info on this! */

/*Task # 1
Give the body element of the site a light blue background using HEX code*/
body {
  background: #0ac6ff;
}

/*Task # 2
Change the h1 to have a 1px solid black border*/
h1 {
  border: solid 1px black;
}

/*Task # 3
Make all h2 elements the color purple*/
h2 {
  color: purple;
}

/*Task # 4
Make all input boxes have a 2px solid dark red border (use rgb for this)*/
input {
  border: solid 2px rgb(255, 10, 10);
}
/*Task # 5
Give a light yellow background to all <p> elements inside of a <div> element
Use HEX for the color*/
div p {
  background: #fff70a;
}
/*Task # 6
There is a textarea element with the id=textblock, give it the following properties:
* A 5px solid gray border
* A width of 800px and a height of 400px
 */
#textblock {
  border: solid 5px gray;
  width: 800px;
  height: 400px;
}
/*Task # 7
There is a link to Google on the page. Make this link red.*/
a {
  color: red;
}

/*Task # 8
Make elements with the id="itemone" have an overline text-decoration.
and be the color purple.*/
#itemone {
  text-decoration: overline;
  color: purple;
}

/*Task # 9
Finally, make the elements with the class label "exit" have
a background of blue and a 4px dashed yellow border.*/
.exit {
  background: blue;
  border: dashed 4px yellow;
}
/*BONUS CHALLENGE: Task 10
There is a link to Google on the page in the list.
Can you figure out how to change the color if you click on the link?
(Hint: Google "css visited") */
a:visited {
  color: greenyellow;
}


// Day 30 October 20. Sunday //

Tempo is going good I am very positive with the overall Front End process... Today I learned about CSS Box Model and to adjust your content with padding,border,margin.
Here is the final assignment... 🥳
#100DaysOfCode 

#top {
  font-family: "Poppins", sans-serif;
  text-align: center;
  margin: auto;
  align-content: center;
}

#cell1 {
  background: #011627;
}

#cell2 {
  background: #70ff28;
}

#cell3 {
  background: #2ec4b6;
}

#cell4 {
  background: #e71d36;
}

#cell5 {
  background: #ff9f1c;
}
table {
  margin: auto;
}

td {
  width: 150px;
  height: 300px;
  border: 6px solid white;
}

// Day 31 October 21. Monday //

Well today I sat down and tried to make a page just to practice my HTML and CSS skills... So I made this replica...
It took me a while but it was worth it... I just have to make the 'Sign me up!' border label like on the image bellow... 
#100DaysOfCode 
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta http-equiv="X-UA-Compatible" content="ie=edge" />
    <link rel="stylesheet" href="CSS_Final.css" />
    <title>Landing Page</title>
  </head>
  <body>
      <!-- <div class="BORDER"> -->
          
    <h1>Welcome to the Landing Page</h1>

    <h2>We're a start-up that does something</h2>
    <div class="Paragraph1">
      <p>
        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Totam soluta
        laboriosam exercitationem architecto expedita recusandae impedit,
        delectus quibusdam sint repudiandae voluptatum atque ea enim cupiditate
        voluptatibus nulla saepe ducimus officiis?
      </p>
    </div>
    <div class="Paragraph2">
      <p>
        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Mollitia magni
        aliquid, dolorem dolore tenetur eaque, ab distinctio nam sapiente eum
        vitae ipsum eligendi. A minima magnam sed recusandae soluta accusantium.
      </p>
    </div>
    <!-- How to make required work ? Should I place all in FORM?-->
    <h2>Sign up for our upcoming launch!</h2>
    <!-- AWESOME !!! THIS WORKS !!! =D -->
    <div class="INPUT">
      <form action="CSS_Final2.html" method="GET">
        <p id="First">First Name:</p>
        <input id="input1" type="text" name="" value="" required />
        <p id="Last">Last Name:</p>
        <input id="input2" type="text" name="" value="" required />
        <p id="Email">Email:</p>
        <input id="input3" type="email" name="useremail" value="" required />
        <!-- I hope this works! It works =D !-->
        <div class="SignIn">
            <input type="submit" name="" value="Sign me up!"
          /></a>
        </div>
      </form>
    </div>
<!-- </div> -->
  </body>
</html>


<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta http-equiv="X-UA-Compatible" content="ie=edge" />
    <link rel="stylesheet" href="CSS_Final.css" />
    <title>Thank you</title>
  </head>
  <body>
    <div class="Thankyou">
      <h3>Thanks for signing up!</h3>
      <h4>We'll reach out to you soon!</h4>
    </div>
  </body>
</html>

/* Need to make the background color and border...but how? 
.BORDER is strange maybe to use background on BODY?*/
/* .BORDER {
  background: black;
  border: 40px solid cadetblue;
} */

body {
  background: black;
  border: 40px solid cadetblue;
}
/* Adjusting the Headers */
/* top , right , bottom , left */

h1 {
  font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
  font-size: 220%;
  color: white;
  text-align: center;
}

h2 {
  font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
  font-size: 150%;
  color: white;
  text-align: center;
}
/* Adjusting the paragraphs */
/* top , right , bottom , left */

.Paragraph1 {
  font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
  font-size: 130%;
  color: white;
  text-align: center;
  width: 40%;
  margin: 10% 30% 5%;
}

.Paragraph2 {
  font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
  font-size: 130%;
  color: white;
  text-align: center;
  width: 40%;
  margin: 5% 30% 5%;
}

/* Adjusting the INPUT */
/* top , right , bottom , left */

.INPUT {
  font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
  color: white;
  text-align: center;
}
#input1 {
  width: 20%;
  padding: 0.65%;
}
#input2 {
  width: 20%;
  padding: 0.65%;
}
#input3 {
  width: 20%;
  padding: 0.65%;
}

#First {
  margin: 0.1%;
}
#Last {
  margin: 0.1%;
}
#Email {
  margin: 0.1%;
}
/* The Thank You Page */
.Thankyou {
  font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
  font-size: 150%;
  color: white;
  text-align: center;
}

/* Adjusting the 'Sign me up!' label */

.SignIn {
  font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
  margin: 1%;
  /* border: 1px solid white; */
}


// Day 32 October 22. Tuesday //
Was reading about Bootstrap Framework and fundamentals ... No code to day sadly because of work ... Tomorrow is a new day...  #100DaysOfCode 

// Day 33 October 23. Wednesday //
Learned about 'Forms' and 'Navbar' with Bootstrap and how to play with them also to make drop-down menus and fixed navbar... It's great to be able to reference a documentation and know what is possible with Bootstrap... 
#100DaysOfCode 
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta http-equiv="X-UA-Compatible" content="ie=edge" />
    <!-- Latest compiled and minified CSS -->
    <link
      rel="stylesheet"
      href="https://stackpath.bootstrapcdn.com/bootstrap/3.4.1/css/bootstrap.min.css"
      integrity="sha384-HSMxcRTRxnN+Bdg0JdbxYKrThecOKuH5zCYotlSAcp1+c8xmyTe9GYg1l9a69psu"
      crossorigin="anonymous"
    />

    <title>NAVBARS</title>
  </head>
  <body>
    <nav class="navbar navbar-default">
      <div class="container">
        <!-- Brand and toggle get grouped for better mobile display -->
    <div class="navbar-header">
            <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#bs-example-navbar-collapse-1" aria-expanded="false">
             <!-- Code for the hamburger icon -->
                <span class="sr-only">Toggle navigation</span>
              <span class="icon-bar"></span>
              <span class="icon-bar"></span>
              <span class="icon-bar"></span>
            </button>
            <a class="navbar-brand" href="#">Brand</a>
          </div>
      
          <!-- Collect the nav links, forms, and other content for toggling -->
          <div class="collapse navbar-collapse" id="bs-example-navbar-collapse-1">
            <ul class="nav navbar-nav">
              <li class="active"><a href="#">Link <span class="sr-only">(current)</span></a></li>
              <li><a href="#">Link</a></li>
              <li class="dropdown">
                <a href="#" class="dropdown-toggle" data-toggle="dropdown" role="button" aria-haspopup="true" aria-expanded="false">Dropdown <span class="caret"></span></a>
                <ul class="dropdown-menu">
                  <li><a href="#">Action</a></li>
                  <li><a href="#">Another action</a></li>
                  <li><a href="#">Something else here</a></li>
                  <li role="separator" class="divider"></li>
                  <li><a href="#">Separated link</a></li>
                  <li role="separator" class="divider"></li>
                  <li><a href="#">One more separated link</a></li>
                </ul>
              </li>
            </ul>
            <form class="navbar-form navbar-left">
              <div class="form-group">
                <input type="text" class="form-control" placeholder="Search">
              </div>
              <button type="submit" class="btn btn-default">Submit</button>
            </form>
            <ul class="nav navbar-nav navbar-right">
              <li><a href="#">Link</a></li>
              <li class="dropdown">
                <a href="#" class="dropdown-toggle" data-toggle="dropdown" role="button" aria-haspopup="true" aria-expanded="false">Dropdown <span class="caret"></span></a>
                <ul class="dropdown-menu">
                  <li><a href="#">Action</a></li>
                  <li><a href="#">Another action</a></li>
                  <li><a href="#">Something else here</a></li>
                  <li role="separator" class="divider"></li>
                  <li><a href="#">Separated link</a></li>
                </ul>
              </li>
            </ul>
        </div>
    </nav>
    <script
  src="https://code.jquery.com/jquery-3.4.1.js"
  integrity="sha256-WpOohJOqMqqyKL9FccASB9O0KwACQJpFTUBLTYOVvVU="
  crossorigin="anonymous"></script>
  <script src="https://stackpath.bootstrapcdn.com/bootstrap/3.4.1/js/bootstrap.min.js" integrity="sha384-aJ21OjlMXNL5UyIl/XNwTMqvzeRMZH2w8c5cRVpzpU8Y5bApTppSuUkhZXN0VxHd" crossorigin="anonymous"></script>
  </body>

</html>


// Day 34 October 24. Thursday //
Just learned about Bootstraps 'Grid System' and the column styling resizing, being able to display correctly whole page structure depending on screen size. Need to practice more... will do an assignment...
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta http-equiv="X-UA-Compatible" content="ie=edge" />
    <link
      rel="stylesheet"
      href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css"
    />
    <title>Document</title>
  </head>

  <style>
    .boxy {
      background: #b3ddff;
      border: 2px solid black;
    }
  </style>

  <div class="container">
    <div class="row">
      <div class="col-lg-4 boxy">COL Large 4</div>
      <div class="col-lg-4 boxy">COL Large 4</div>
      <div class="col-lg-4 boxy">COL Large 4</div>
    </div>
  </div>
  <div class="container">
    <div class="row">
      <div class="col-md-6 boxy">COL Med 6</div>
      <div class="col-md-6 boxy">COL Med 6</div>
    </div>
  </div>

  <!-- <div class="container">
    <div class="row">
      <div class="col-lg-3 col-sm-6 boxy">ONE</div>
      <div class="col-lg-3 col-sm-6 boxy">TWO</div>
      <div class="col-lg-3 col-sm-6 boxy">THREE</div>
      <div class="col-lg-3 col-sm-6 boxy">FOUR</div>
    </div>
  </div>

  <!-- <div class="row">
    <div class="col-lg-6 boxy">
      <div class="row">
        <div class="col-lg-6 boxy">NEST ONE</div>
        <div class="col-lg-6 boxy">NEST TWO</div>
      </div>
    </div>
    <div class="col-lg-6 boxy">TOP LEVEL</div>
  </div> -->

  <body></body>
</html>


#100DaysOfCode 

// Day 35 October 25. Friday //

Today I tried to do a Bootstrap web project, got so much to do will finish tomorrow... All in all I am very happy with the progress. Oh and yes I am a Tea guy lol. 🍵 
#100DaysOfCode
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta http-equiv="X-UA-Compatible" content="ie=edge" />
    <link
      rel="stylesheet"
      href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css"
    />
    <title>Tea Lover Project</title>
  </head>
  <body>
    <nav class="navbar navbar-default navbar-dark bg-dark">
      <a class="navbar-brand" href="#">Welcome</a>
      <button
        class="navabar-toggler bg-dark"
        type="button"
        data-toggle="collapse"
        data-target="#navbarSupportedContent"
        aria-controls="navbarSupportedContent"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav mr-auto">
          <li class="nav-item active">
            <a class="nav-link" href="#"
              >Home <span class="sr-only">(current)</span></a
            >
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Link</a>
          </li>
          <li class="nav-item dropdown">
            <a
              class="nav-link dropdown-toggle"
              href="#"
              id="navbarDropdown"
              role="button"
              data-toggle="dropdown"
              aria-haspopup="true"
              aria-expanded="false"
            >
              Dropdown
            </a>
            <div class="dropdown-menu" aria-labelledby="navbarDropdown">
              <a class="dropdown-item" href="#">Action</a>
              <a class="dropdown-item" href="#">Another action</a>
              <div class="dropdown-divider"></div>
              <a class="dropdown-item" href="#">Something else here</a>
            </div>
          </li>
          <li class="nav-item">
            <a
              class="nav-link disabled"
              href="#"
              tabindex="-1"
              aria-disabled="true"
              >Disabled</a
            >
          </li>
        </ul>
        <form class="form-inline my-2 my-lg-0">
          <input
            class="form-control mr-sm-2"
            type="search"
            placeholder="Search"
            aria-label="Search"
          />
          <button class="btn btn-outline-success my-2 my-sm-0" type="submit">
            Search
          </button>
        </form>
      </div>
    </nav>
    <div class="container">
      <div class="jumbotron">
        <h1>Tea Lover Project</h1>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Ea suscipit
          iure minus quaerat optio, voluptates voluptate tenetur velit ipsam
          atque itaque aliquam libero eius eaque. Quasi exercitationem inventore
          incidunt magnam.
        </p>
        <a class="btn btn-primary btn-lg" href="#" role="button">Learn more</a>
      </div>
      <p>
        Lorem ipsum dolor, sit amet consectetur adipisicing elit. Culpa
        consectetur ratione obcaecati, perferendis quod aliquam sequi facere sed
        incidunt harum aliquid magni aut? Maiores aperiam sed odit fugiat vitae
        aliquid.
      </p>
      <p>
        Lorem ipsum dolor, sit amet consectetur adipisicing elit. Earum quo
        ullam alias! Non, laboriosam? Rem error nesciunt dignissimos eum illum
        officia fugit. Inventore aut assumenda illo dolorem temporibus doloribus
        aliquam!
      </p>
    </div>
    <script
      src="https://code.jquery.com/jquery-3.4.1.js"
      integrity="sha256-WpOohJOqMqqyKL9FccASB9O0KwACQJpFTUBLTYOVvVU="
      crossorigin="anonymous"
    ></script>
    <script
      src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.7/umd/popper.min.js"
      integrity="sha384-UO2eT0CpHqdSJQ6hJty5KVphtPhzWj9WO1clHTMGa3JDZwrnQq4sF86dIHNDz0W1"
      crossorigin="anonymous"
    ></script>
  </body>
</html>

// Day 36 October 26. Saturday //

Finally Bootstrap project done... I have learned a ton of things especially the grid and columns formation and how its important to customize for certain device screen size... I am very proud and happy of my progress... 🤓💻💪
#100DaysOfCode 
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta http-equiv="X-UA-Compatible" content="ie=edge" />
    <link
      rel="stylesheet"
      href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css"
    />
    <title>Tea Lover Project</title>
  </head>
  <body>
    <!-- NAVBAR with link to another page -->
    <!-- As a heading -->
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
      <a class="navbar-brand" href="#">Welcome</a>
      <!-- HAMBURGER -->

      <button
        class="navbar-toggler"
        type="button"
        data-toggle="collapse"
        data-target="#bs-example-navbar-collapse-1"
        aria-controls="bs-example-navbar-collapse-1"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>

      <!-- SIGN IN PAGE -->
      <div class="collapse navbar-collapse" id="bs-example-navbar-collapse-1">
        <div class="navbar-nav">
          <a
            class="nav-item nav-link"
            href="D:\SOFTWARE DEV\My_project\CSS\Bootstrap_project_login.html"
            >Sign In</a
          >
        </div>
      </div>
    </nav>

    <!-- JUMBOTRON BODY -->
    <div class="container">
      <div class="jumbotron">
        <h1>Tea Lover Project</h1>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Ea suscipit
          iure minus quaerat optio, voluptates voluptate tenetur velit ipsam
          atque itaque aliquam libero eius eaque. Quasi exercitationem inventore
          incidunt magnam.
        </p>
      </div>
      <p>
        Lorem ipsum dolor, sit amet consectetur adipisicing elit. Culpa
        consectetur ratione obcaecati, perferendis quod aliquam sequi facere sed
        incidunt harum aliquid magni aut? Maiores aperiam sed odit fugiat vitae
        aliquid.
      </p>
      <p>
        Lorem ipsum dolor, sit amet consectetur adipisicing elit. Earum quo
        ullam alias! Non, laboriosam? Rem error nesciunt dignissimos eum illum
        officia fugit. Inventore aut assumenda illo dolorem temporibus doloribus
        aliquam!
      </p>
      <!-- Pictures of Tea grid system -->
      <h2>Pictures of Tea</h2>
      <div class="container">
        <div class="row">
          <div class="col-lg-4 col-6 px-0">
            <img
              src="https://cdn.stocksnap.io/img-thumbs/960w/S85GWDUCE4.jpg"
              alt=""
              class="img-thumbnail"
            />
          </div>
          <div class="col-lg-4 col-6 px-0">
            <img
              src="https://cdn.stocksnap.io/img-thumbs/960w/0ZS74TCOME.jpg"
              alt=""
              class="img-thumbnail"
            />
          </div>
          <div class="col-lg-4 col-6 px-0">
            <img
              src="https://cdn.stocksnap.io/img-thumbs/960w/QQHVJIP0IJ.jpg"
              alt=""
              class="img-thumbnail"
            />
          </div>
          <div class="col-lg-4 col-6 px-0">
            <img
              src="https://cdn.stocksnap.io/img-thumbs/960w/R28VJEGM5B.jpg"
              alt=""
              class="img-thumbnail"
            />
          </div>
          <div class="col-lg-4 col-6 px-0">
            <img
              src="https://cdn.stocksnap.io/img-thumbs/960w/QJGCG8IAEZ.jpg"
              alt=""
              class="img-thumbnail"
            />
          </div>
          <div class="col-lg-4 col-6 px-0">
            <img
              src="https://cdn.stocksnap.io/img-thumbs/960w/1OBXVC1ARF.jpg"
              alt=""
              class="img-thumbnail"
            />
          </div>
        </div>
      </div>
    </div>
    <script
      src="https://code.jquery.com/jquery-3.3.1.slim.min.js"
      integrity="sha384-q8i/X+965DzO0rT7abK41JStQIAqVgRVzpbzo5smXKp4YfRvH+8abtTE1Pi6jizo"
      crossorigin="anonymous"
    ></script>
    <script
      src="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/js/bootstrap.min.js"
      integrity="sha384-ChfqqxuZUCnJSK3+MXmPNIyE6ZbWh2IMqE241rYiqJxyMiZ6OW/JmZQ5stwEULTy"
      crossorigin="anonymous"
    ></script>
  </body>
</html>


<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta http-equiv="X-UA-Compatible" content="ie=edge" />
    <link
      rel="stylesheet"
      href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css"
    />
    <title>Sign In</title>
  </head>
  <body>
    <!-- NAVBAR with link to another page -->
    <!-- As a heading -->
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
      <a
        class="navbar-brand"
        href="D:\SOFTWARE DEV\My_project\CSS\Bootstrap_project.html"
        >Welcome</a
      >
      <!-- HAMBURGER -->
      <button
        class="navbar-toggler"
        type="button"
        data-toggle="collapse"
        data-target="#bs-example-navbar-collapse-1"
        aria-controls="bs-example-navbar-collapse-1"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <!-- HOME PAGE -->
      <div class="collapse navbar-collapse" id="bs-example-navbar-collapse-1">
        <div class="navbar-nav">
          <a
            class="nav-item nav-link"
            href="D:\SOFTWARE DEV\My_project\CSS\Bootstrap_project.html"
            >Home</a
          >
        </div>
      </div>
    </nav>
    <!-- JUMBOTRON BODY -->
    <div class="container">
      <div class="jumbotron">
        <h1>Log In</h1>
        <p>Enter your email and password below to log in to Tea Lover</p>
      </div>
    </div>
    <div class="container">
      <form>
        <div class="form-group">
          <label for="exampleInputEmail1">Email address</label>
          <input
            type="email"
            class="form-control"
            id="exampleInputEmail1"
            placeholder="Email"
            required
          />
        </div>
        <div class="form-group">
          <label for="exampleInputPassword1">Password</label>
          <input
            type="password"
            class="form-control"
            id="exampleInputPassword1"
            placeholder="Password"
            required
          />
        </div>
        <div class="checkbox">
          <label> <input type="checkbox" /> Keep me Logged In </label>
        </div>
        <button type="submit" class="btn btn-secondary">Submit</button>
      </form>
    </div>
    <script
      src="https://code.jquery.com/jquery-3.3.1.slim.min.js"
      integrity="sha384-q8i/X+965DzO0rT7abK41JStQIAqVgRVzpbzo5smXKp4YfRvH+8abtTE1Pi6jizo"
      crossorigin="anonymous"
    ></script>
    <script
      src="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/js/bootstrap.min.js"
      integrity="sha384-ChfqqxuZUCnJSK3+MXmPNIyE6ZbWh2IMqE241rYiqJxyMiZ6OW/JmZQ5stwEULTy"
      crossorigin="anonymous"
    ></script>
  </body>
</html>

// Day 37 October 27. Sunday //

Today I just took an introduction to Javascript reading about adding interaction functionality to websites... It will be very cool to make something with JS and I cant wait...🤓💪💻
#100DaysOfCode 

// Day 38 October 28. Monday //

Day 37 
Ok I went through Javascript basics and I laughed when I found out it was actually in Chrome the whole time I though I had to Install separatelly lol. Anyway I was doing basic data types, strings, booleans, math, string concatenation, indexing and var's. 
#100DaysOfCode 
VM546:1 Console was cleared
undefined
2+2
4
5-1
4
3*2
6
10/2
5
2/5
0.4
"Django" + " " + "is super cool."
"Django is super cool."
"django".lenght
undefined
"django".length
6
"hello \n start a new line"
"hello 
 start a new line"
"hello"[4]
"o"
"look at the dog"[12]
"d"
var bankAccount = 100:
VM1048:1 Uncaught SyntaxError: Unexpected token ':'
var bank
undefined
var bankAccount = 100;
undefined
bankAccount
100
var deposit = 50;
undefined
var total = bankAccount + deposit
undefined
total
150
var greeting = "Welcome back: ";
undefined
var name = "Emin";
undefined
alert()
undefined
alert(greeting + name)
undefined
alert(greeting + name)
undefined
alert("HEY!")
undefined
console.log("hey im in the console")
VM1644:1 hey im in the console
undefined
prompt("Enter something")




// Day 39 October 29. Tuesday //

A very busy day it was... Tired ... Managed to look at some Javascript and how to connect it to an HTML file...I know nothing thats lame.. but I really need to sleep... tomorrow I'll crunch the heck out of Javascript I promise... 😷🛌🤘
#100DaysOfCode 

<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta http-equiv="X-UA-Compatible" content="ie=edge" />
    <title>Document</title>
    <script src="myscript.js"></script>
  </head>
  <body>
    <h1>Welcome to your bank!</h1>
  </body>
</html>

alert('Welcome to your bank');
var deposit = prompt('How much would you like to deposit today?');
alert('Youve deposited: ' + deposit);
console.log('You are a cool person!');



// Day 40 October 30. Wednesday //
So today I red through JS syntax operators, control flow... I have already learned about if statements, booleans and other stuff while learning python so I think I will skim through the JS part till projects part...
#100DaysOfCode 
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <script src="myscript2.js"></script>
    <meta http-equiv="X-UA-Compatible" content="ie=edge" />
    <title>Document</title>
  </head>
  <body></body>
</html>

var ham = 0;
var cheese = 0;

var report = 'blank';

if (ham >= 10 && cheese >= 10) {
  report = 'Strong sales of both ham and cheese!';
} else if (ham === 0 && cheese === 0) {
  report = 'Nothing sold';
} else {
  report = 'We had some sales of items.';
}
console.log(report);


// Day 41 October 31. Thursday //
Today I did some exercises "while loops" and "for loops"...
For tomorrow I will be doing a little project just to summarize the basics... Now its horror movie time... 😈👻💀☠️👽
#100DaysOfCode 
/// PART 8 - LOOP EXERCISES
// Before we continue on with your project, let's practice some loops!
// You'll have just two problems, but you'll need to use each loop type we
// learned about to solve them!

///////////////////
//// PROBLEM 1 ///
/////////////////

// Use a For Loop to print (console.log()) out the word "hello" 5 times.
//
// Do this with a While Loop and a For Loop

// While Loop

var x = 0;
var word = "hello";

while (x < 5) {
    console.log(word);
    x = x + 1;
}

// For Loop

for (var i = 0; i < 5; i++) {
    console.log("hello with for loop");

}

/////////////////
// PROBLEM 2 ///
///////////////

// Use Loops to console.log() (print out) all the odd numbers from 1 to 25
// Do this using two methods, a while loop and a for loop

// METHOD ONE
// While Loop

var num = 1;

while (num<25){
    if (num%2 ! == 0) {
        console.log(num);

    }
    num++
}

// METHOD TWO
// For Loop

for (var i = 0; i < 5; i++ ) {
    if (i%2 !== 0){
        console.log(i);

    }
}



// Day 42 November 01. Friday //

Today I did a JavaScript lvl 1 project. I know I could have skipped this chapter since I already learned in python but I will finish the chapter probably tomorrow with a project. After that I have DOM and jQuery to tackle in order to advance to Back-End.
#100DaysOfCode 

alert('Restricted Government Access! Please input your information!');

var first_name = prompt('Please add your first name.');
alert('Your first name is' + ' ' + first_name);
var last_name = prompt('Please add your last name.');
alert('Your last name is' + ' ' + last_name);
var age = prompt('Please add your age number.');
alert('Your are' + ' ' + age + ' ' + 'years old.');
var height = prompt('Please add your height in cm.');
alert('Your height is' + ' ' + height + ' ' + 'cm.');
var pet = prompt('Please add your pets name.');
alert('Your pets name is' + ' ' + pet + '.');

var nameCond = null;
var ageCond = null;
var heightCond = null;
var petCond = null;

if (first_name[0] === last_name[0]) {
  nameCond = true;
} else {
  nameCond = false;
}

if (age > 50 && age < 70) {
  ageCond = true;
} else {
  ageCond = false;
}

if (height >= 170) {
  heightCond = true;
} else {
  heightCond = false;
}

if (pet[pet.length - 1] === 'y') {
  petCond = true;
} else {
  petCond = false;
}

if (nameCond && ageCond && heightCond && petCond) {
  report = 'ACCESS GRANTED!';
} else {
  report = 'ACCESS DENIED!';
}
console.log(report);

// if (
//   first_name === 'Tom' &&
//   last_name === 'Travolta' &&
//   age === '65' &&
//   height === '189' &&
//   pet === 'Johnny'
// ) {
//   report = 'ACCESS GRANTED!';
// } else {
//   report = 'ACCESS DENIED!';
// }
// console.log(report);


// Day 43 November 02. Saturday //

Well today I've went through Javascript_lvl_two chapter doing some simple problems with 'functions','arrays', and 'objects'... So far I prefer Python and will stick to it in the future... Anyway tomorrow will continue with DOM chapter.
💻🤓
#100DaysOfCode 

// Day 44 November 05. Tuesday //

Now I took a look on that DOM chapter and I must say now it all makes sense of the front-end structure... I really like the "event listeners" function... Will do a simple project tomorrow... 🤓💻#100DaysOfCode 
var headOne = document.querySelector('#one');
var headTwo = document.querySelector('#two');
var headThree = document.querySelector('#three');

headOne.addEventListener('mouseover', function() {
  headOne.textContent = 'Mouse Currently Over';
  headOne.style.color = 'red';
});

headOne.addEventListener('mouseout', function() {
  headOne.textContent = 'HOVER OVER ME';
  headOne.style.color = 'black';
});

headTwo.addEventListener('click', function() {
  headTwo.textContent = 'CLICKED ON';
  headTwo.style.color = 'blue';
});

headThree.addEventListener('dblclick', function() {
  headThree.textContent = 'I WAS DOUBLE CLICKED!';
  headThree.style.color = 'red';
});

//Day 45 November 06. Wednesday//
A awesome day today!
I just made TicTacToe using the DOM methods... I know as a beginner  I will mostly code in DRY but this is the only way to get to CLEAN later on haha... Persistence is key... Anyway tomorrow will be focusing on jQuery...💪
#100DaysOfCode 
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta http-equiv="X-UA-Compatible" content="ie=edge" />
    <link rel="stylesheet" href="tictactoe.css" />
    <link
      rel="stylesheet"
      href="https://stackpath.bootstrapcdn.com/bootstrap/3.4.1/css/bootstrap.min.css"
      integrity="sha384-HSMxcRTRxnN+Bdg0JdbxYKrThecOKuH5zCYotlSAcp1+c8xmyTe9GYg1l9a69psu"
      crossorigin="anonymous"
    />
    <title>GAME ON!</title>
  </head>
  <body>
    <!-- JUMBOTRON HEADER -->
    <div class="container">
      <div class="jumbotron">
        <h1>Welcome to Tic Tac Toe!</h1>
        <a id="b" class="btn btn-primary btn-lg" href="#" role="button"
          >Restart!</a
        >
      </div>
    </div>
    <!-- BORDER GRID -->
    <div class="container">
      <table class="table">
        <tr>
          <td id="one"></td>
          <td id="cell"></td>
          <td id="cell"></td>
        </tr>
        <tr>
          <td id="cell"></td>
          <td id="cell"></td>
          <td id="cell"></td>
        </tr>
        <tr>
          <td id="cell"></td>
          <td id="cell"></td>
          <td id="cell"></td>
        </tr>
      </table>
    </div>

    <script
      src="https://code.jquery.com/jquery-3.4.1.js"
      integrity="sha256-WpOohJOqMqqyKL9FccASB9O0KwACQJpFTUBLTYOVvVU="
      crossorigin="anonymous"
    ></script>
    <script
      src="https://stackpath.bootstrapcdn.com/bootstrap/3.4.1/js/bootstrap.min.js"
      integrity="sha384-aJ21OjlMXNL5UyIl/XNwTMqvzeRMZH2w8c5cRVpzpU8Y5bApTppSuUkhZXN0VxHd"
      crossorigin="anonymous"
    ></script>
  </body>
  <script src="Game.js"></script>
</html>

//Restart game button
var restart = document.querySelector('#b');
//Grabs all the squares
var squares = document.querySelectorAll('td');

//Clear all the squares
function clearBoard() {
  for (var i = 0; i < squares.length; i++) {
    squares[i].textContent = '';
  }
}

restart.addEventListener('click', clearBoard);
//Check the square marker

//1. This is DRY method which I should avoid
// var cellOne = document.querySelector('#one');
// cellOne.addEventListener('click', function() {
//   if (cellOne.textContent === '') {
//     cellOne.textContent = 'X';
//   } else if (cellOne.textContent === 'X') {
//     cellOne.textContent = 'O';
//   } else {
//     cellOne.textContent = '';
//   }
// });

// 2. The CLEAN correct best way
function changeMarker() {
  if (this.textContent === '') {
    this.textContent = 'X';
  } else if (this.textContent === 'X') {
    this.textContent = 'O';
  } else {
    this.textContent = '';
  }
}

//For Loop to add event Listener to all the squares
for (let i = 0; i < squares.length; i++) {
  squares[i].addEventListener('click', changeMarker);
}
// var cell = document.querySelector('#cell');
// cell.addEventListener('click', function() {
//   cell.textContent = 'X';
// });
// cell.addEventListener('dblclick', function() {
//   cell.textContent = 'O';
// });
console.log('Connected!');

table {
  border: 6px solid black;
  width: 150px;
  height: 150px;
  text-align: center;
  font-size: 80px;
}

tr {
  border: 6px solid black;
  width: 150px;
  height: 150px;
  text-align: center;
}

td {
  border: 6px solid black;
  width: 150px;
  height: 150px;
  text-align: center;
}


//Day 46 November 07. Thursday//

Just did the basics of jQuery grabbing text in HTML, attributes,values and classes... It really does simplify your workflow since its basically a javascript library with many pre-built methods and objects... Tomorrow will be doing a little exercise... 🤘
#100DaysOfCode

//Day 47 November 08. Friday//
Big announcement folks ! I just finished with the front-end part! 🤗 Moving now to Back-end and will be using Python & Django... I am really excited and cant wait to make amazing stuff... 💪🤘💻🤓 
#100DaysOfCode 

//Day 48 November 10. Sunday//
Just skimmed through Python basics and did some coding exercises, gonna do some more tomorrow before jumping to Django... 🤗🤘💻
import random

# Get Guess
def get_guess():
    return list(input("What is your guess"))


# Generate computer code 123
def generate_code():
    digits = [str(num) for num in range(10)]

    # shuffle the digits
    random.shuffle(digits)
    # Then grab the first three
    return digits[:3]


# Generate the clues
def generate_clues(code, user_guess):
    if user_guess == code:
        return "CODE CRACKED!"

    clues = []

    for ind, num in enumerate(user_guess):
        if num == code[ind]:
            clues.append("match")
        elif num in code:
            clues.append("close")

    if clues == []:
        return ["Nope"]
    else:
        return clues


# run game logic
print("Welcome Code Breaker!")

secret_code = generate_code()

clue_report = []

while clue_report != "CODE CRACKED!":
    guess = get_guess()

    clue_report = generate_clues(guess, secret_code)
    print("here is the result of your guess:")
    for clue in clue_report:
        print(clue)

#100DaysOfCode


//Day 49 November 11. Monday//
Was going through OOP (Object Oriented Programming) just to understand it better and  skimmed through 'Attributes and Methods ' plus the 'Inheritance & special methods' will need to do more exercises.
#100DaysOfCode 
class Book:
    def __init__(self, title, author, pages):
        self.title = title
        self.author = author
        self.pages = pages

    # special method
    def __str__(self):
        return "Title: {}, Author: {}, Pages: {}".format(self.title, self.author, self.pages)

    def __len__(self):
        return self.pages

    def __del__(self):
        print("a book is destroyed!")


b = Book("Python", "Emin", 200)
del b

//Day 50 November 12. Tuesday//
A busy day it was going through python 'Errors and exception' + ' modules and packages'...
Finally I am ready to take my first lesson on Django framework for the back-end part... I AM THE BEST !!! 💪🤣💻
#100DaysOfCode

//Day 51 November 14. Thursday//
Took me whole day to setup conda virtual environment via vscode installing packages Django through conda and pip, rewiring paths for integrated terminal... pfff ... it was a maze... I believe I have setup one venv correctly. All in all Django awaits ! 😷🤖
#100DaysOfCode 

//Day 52 November 15. Friday//
Created my first Django application and learned about "Views" and how to use them... Awesome day ... 🤣💻
#100DaysOfCode 

//Day 53 November 16. Saturday//
Did a challenge task of creating a new project and Django app, learned how to run the server. As I see there is a difference between using a string of html code instead of a normal string.🙂
#100DaysOfCode

//Day 54 November 17. Sunday //
Learned today about Django - Url Mapping and the ability of using the 'include()' function to keep projects clean and modular. After that learned about Django - Templates and I do now have a basic understanding of how Django works... 
#100DaysOfCode 

//Day 55 November 20. Wednesday //

Learned about static files in Django - and did a summary project Url Mapping, template and static files, had an issue adding template tags since the jpg image wasn't showing up... Will review it again just to mind map it... Next will be 'Models'. 
#100DaysOfCode 

//Day 56 November 22. Friday //

Today I was learning about Django "Models" and I have to say it is awesome to see something built completely with just a few lines of code + SQL databases ( in this case heres an admin page)... Django is powerfull ! 💪
#100DaysOfCode

//Day 57 November 23. Saturday //

Sometimes its good to make a script to populate your models with some "fake" data... So I learned about Django - Population Script "FAKER" and its library, it really is a cool thing to have. lol 🤣🤘
#100DaysOfCode

//Day 58 November 26. Tuesday //

After learning about how Django operates what is known as Models-Templates-Views, my goal was to learn how to connect everything. To practice this I have started with generating a table. And then I ran into a problem. Posted on Stack Overflow. 🧐Sherlock
#100DaysOfCode 

//Day 59 December 01. Sunday //

Finally solved the issues after punishing hours and lack of sleep. Table connection and other Django import features now work... Had to check VS Code extensions and also Django documentation... Now I can continue my journey normally... NEVER GIVE UP !🤕💪
#100DaysOfCode
