# python
# a single line comment in python like in bash !like in sql || CSharp
''' '''
This is a multiline
comment.
''' '''


import all math operations
import sys
import os
import random
from math import *

#text
print("Hello ")
print ("Welcom to a | \n  \" \' \f \e \a \b \c \d \d a Basic python code")
print("  *  ")
print(" * * ")
print("* * *")
text="Var"
print (text +" : ")
print (text.lower())
print (text.upper())
print (text.isupper())
print (text.upper().isupper())
print ("text length : "+ str(len(text)))
print (text[0] +" is the first character")
print (str(text.index("V")) +" is the index of V in "+ text)
print (str(text.index("Va")) +" is the index of Va in "+ text)
print(text.replace("V","C"))

#numbers
print (3 + 4.5)
print (-1*-2.29008850)
print (3*(3*6))
print (10%3)
a=3
b=2
print (str(a+b))
a=a+b
b=a-b
a=a-b
print(a)
print(b)
print (pow(a,2))
print(max(a,b))
print (min(a,b))
print(round(3.157,2))
print (floor(3.75))
print (ceil(3.75))
print (sqrt(36))

#inputs

name=input("Please enter your name: ")
age=input("Age please: ")
print ("Welcome "+name +" you are : "+age)

num1 = input ("Number 1:")
num2 = input("Number 2:")
SumInt=int(num1)+int(num2)
Sumfloat=float(num1)+float(num2 )

print (str(SumInt) +"  " +str(Sumfloat))


#Lists
lucky_numbers=[40,50,70,62]
friends=["Youssef","Amine","AbdElmonim","Soufiane"]
print(["Hello " + str(friend) for friend in friends] )
print ("--")
print (friends[0])
print (friends[1:3])
friends.extend(lucky_numbers)
print([str(friend) for friend in friends] )

friends=["Youssef","Amine","AbdElmonim","Soufiane"]

friends.sort()
print([str(friend) for friend in friends] )
friends.append("Mohamed")
print([str(friend) for friend in friends] )
friends.insert(1,"Mohamed")
print([str(friend) for friend in friends] )
friends.remove("Soufiane")
print([str(friend) for friend in friends] )
friends.pop() #remove last element
print([str(friend) for friend in friends] )
friendsReverse=friends.copy()
friendsReverse.reverse()
print([str(friend) for friend in friendsReverse] )
print(friendsReverse.count("Mohamed"))
friends.clear()
print([str(friend) for friend in friends] )

for friend in lfriends
    print("Salam " + friend +"\n")


#Tuples | Fixed list > changes are not allowed
coordinates=(4.552120,52.12222154)
print(coordinates[0])

#list of tuples
coordinates=[(3,1),(5,6),(9,0)]
print(coordinates[1][1])

#functions
def _Function_():
    print("this helllooooo is printed ")
    return False
print("this helloo will not be a part of the code")
print ("because the indent (la tabulation) is not present => function end :)")

returned=_Function_()
print(returned)

def _func_(A, B):
    print(A+B)
_func_(3, 5)
def _func_(Age, B):
    print(str(Age)+" is the age of:"+B)
_func_(21, "Mohamed")

#if statements
print("When I wake up")
hungry=True
ramadan=True
if hungry and not(ramadan):
   print("I eat breakfast")
   print("Wohooo :D")
elif hungry and ramadan:
    print ("It's Ramadan Bro :D")
else:
   print("just eat that breakfast")

def Maxnum(a,b,c):
    if a>=b and a>=c :
        return a
    elif  b>=a and b>=c:
        return b
    else:
        return c
print(Maxnum(3,4,5))


#Dictionnaires Key,Value
Months={
    "Jan":"January",
    "Feb":"February",
    "Mar":"March",
}
print(Months["Jan"])
print(Months.get("Dec","Month not in dictionnary"))

# random
# import random
rand=random.randrange(0,100)

#While loop :P

text=""
while True:
    text+="."
    print(text)
    
#for loops
    for y in [1,2,3,4,5,6,7,8,9]
        print(y)
    for x in range(0,3)
        for y in range (0,3)
            print ("("+ x +" ,"+y+")")


#files
>import os

##Make
testfile=open("text.txt","wb")
print(testfile.mode)
print(testfile.name)
testfile.write(bytes(" Write me to the file \n Hey hhhh",'UTF-8'))
testfile.close()

##Open
testfile=open("text.txt","r+")
Textinfile=testfile.read()
print(Textinfile)
testfile.close()

##Delete
os.remove("text.txt")

#Objects
class Animal:
    __name=""
    __height=0
    __weight=0
    __sound=0
    def __init__(self, name, height, weight,sound):
        self.__name=name
        self.__height=height
        self.__weight=weight
        self.__sound=sound
    def setname(self,name):
        self.__name=name
    def getname(self):
        return self.__name
    def setheight(self,height):
        self.__height=height
    def getheight(self):
        return self.__height
    def setweight(self,weight):
        self.__weight=weight
    def getweight(self):
        return self.__weight
    def setsound(self,sound:
        self.__sound=sound
    def getsound(self):
        return self.__sound
    def get_type(self):
        return "Animal"
    def toString(self):
        return "Data > name:{0},height: {1} cm,weight: {2}Kg,sound: {3}".format(self.__name,self.__height,self.__weight,self.__sound)
cat = Animal('Sami',33,10,'Meeeo')
print(cat.toString())

#Heritage
class Dog(Animal):
    __owner=""
    def __init__(self, name, height, weight, sound, owner):
        self.__owner=owner
        super(Dog, self).__init__(,ame,height,weight,sound)
    def set_owner(self,owner):
        self.__owner=owner
    def get_owner(self):
        return self.__owner
    def toString(self):
        return "Data > name: {},height: {} cm,weight: {}Kg,sound: {},  Owner: {}".format(self.__name, self.__height,self.__weight, self.__sound, self.__owner)
    def multi_sound(self, howmay=None):
        if howmany is None:
            print(self.get_sound())
        else:
            print(self.get_sound()*howmany)
dog= Dog("Rex",800,30,"HwHw","Jack")
print(dog.toString())
