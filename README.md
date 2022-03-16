# CodeWars_Py.Solved_solutions
Pg- 1
Timmy & Sarah think they are in love, but around where they live, they will only know once they pick a flower each. If one of the flowers has an even number of petals and the other has an odd number of petals it means they are in love.
Write a function that will take the number of petals of each flower and return true if they are in love and false if they aren't.

#### My Solution:

def lovefunc( flower1, flower2 ):     
    return (flower1 + flower2) % 2 != 0
    
#### Another understandable way :
def lovefunc( flower1, flower2 ):     
    if (flower1+flower2 )%2==0:
        return False
    elif (flower1+flower2 )%2!=0:
        return True
Pg- 2:     
#Description:
#In this simple assignment you are given a number and have to make it negative. But maybe the number is already negative?

#Example:

#makeNegative(1); return -1
#makeNegative(-5); return -5
#makeNegative(0); return 0
#Notes:

#The number can be negative already, in which case no change is required.
#Zero (0) can't be negative, see examples above.

#### My Solution:
def make_negative(number):
    if number > 0:
        return number * -1
    elif number < 0:
        pass
    return number
    
    or
    
def make_negative(number):
    if number > 0:
        return -number
    elif number < 0:
        pass
    return number

Pg- 3:
The code does not execute properly. Try to figure out why ?

function multiply(a, b)
    a * b

#### My Solution:

function multiply(a, b)
   return a * b
   
Pg- 4:  
#### Exclamation marks series #11: Replace all vowel to exclamation mark in the sentence
Replace all vowel to exclamation mark in the sentence. aeiouAEIOU is vowel.

#### My Solution:




Pg- 5:
#### Find the smallest integer in the array

    Given an array of integers your solution should find the smallest integer. For example:

    Given [34, 15, 88, 2] your solution will return 2
    Given [34, -345, -1, 100] your solution will return -345
    
#### My Solution:




Pg- 6:
Very simple, given an integer or a floating-point number, find its opposite.
Examples:

1: -1
14: -14
-34: 34

#### My Solution:

def opposite(number):
  return number*-1
  
  
Pg- 7:
Our football team finished the championship. The result of each match look like "x:y". Results of all matches are recorded in the collection.
For example: ["3:1", "2:2", "0:1", ...]

Write a function that takes such collection and counts the points of our team in the championship. Rules for counting points for each match:

    if x>y - 3 points
    if x<y - 0 point
    if x=y - 1 point
Notes:
    there are 10 matches in the championship
    0 <= x <= 4
    0 <= y <= 4

#### My Solution:

def points(games):
    s=[]
    for items in games:
        items = items.split(":")
        if items[0] > items[1]:
            s.append(3)
        elif items[0] == items[1]:
            s.append(1)
    return sum(s) 
    
