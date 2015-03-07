footer: © [Tasos Sangiotis](http://tsangiotis.com), [IEEE SB UPatras](http://ieee-upatras.gr), 2015

![inline 60%](python-logo.png)

# An Introduction

---

Η Python είναι μία δυναμική και ερμηνευτική γλώσσα προγραμματισμού.

Δεν υπάρχουν δηλώσεις τύπων με αποτέλεσμα ο κώδικας να είναι σύντομος και ευέλικτος.

Όλα γίνονται στην εκτέλεση.
Αν υπάρχει κάποιο κομμάτι κώδικα που δε βγάζει νόημα το πρόγραμμα θα τρέξει μέχρι να φτάσει εκεί.

---
#Hello World!

```Python
>>> print "Hello, World!"
```

---
#Απλά Μαθηματικά

```Python
>>> 1 + 1
2
>>> 6-5
1
>>> 2*5
10
>>> 5**2 #5 στο τετράγωνο
25
>>> 21/3
7
>>> 23/3
7
>>> 23.0/3.0
7.6666...
>>> 23%3
2
(Υπόλοιπο Ευκλείδιας Διαίρεσης/Modulo)
```

---
#Απλά Μαθηματικά

```Python
>>> print "1 + 2 is an addition"
1 + 2 is an addition
(Απλά γράφουμε κάτι στην οθόνη)
>>> print "one kilobyte is 2^10 bytes, or", 2**10, "bytes"
one kilobyte is 2^10 bytes, or 1024 bytes
(Μπορούμε να τυπώσουμε αποτελέσματα πράξεων και
  μεταβλητές μέσα σε μια πρόταση.
Τα κόμματα διαχωρίζουν κάθε κομμάτι
  είναι ένας τρόπος να διαχωρίζουμε τι τυπώνουμε.)
```

#Απλά Μαθηματικά

```Python
>>> 1 + 2 * 3
7
>>> (1 + 2) * 3
9
```

---
![](obama-code.jpg)

#Let's get Serious!
###Μαζί με τον Ομπάμα!:+1:


---
![inline 40%](pascal_logo.png) vs ![inline 60%](python-logo.png)

Με ένα απλό παράδειγμα

---
Pascal:


```Delphi
Program Program1;
Var
    Num1, Num2, Sum : Integer;

Begin {no semicolon}
 Write('Enter first number: ');
 Readln(Num1);
 Writeln('Enter second number: ');
 Readln(Num2);
 Sum := Num1 + Num2; {addition}
 Writeln(Sum);
 Readln;
End.
```

---
#Ένα πρόγραμμα που:
1. Διαβάζει 2 αριθμούς
2. Προσθέτει τους 2 αριθμούς
3. Εμφανίζει το αποτέλεσμα της πρόσθεσης.

###Hint:

```Python
>>> myName = input('What is your name: ')
What is your name: Tasos
>>> print (myName)
Tasos
```

---
Python:

```Python
num1 = input('Enter first number: ')
num2 = input('Enter second number: ')
sum = num1 + num2
print(sum)
```

---
#Σχόλια

Μία πάρα πολύ καλή συνήθεια.

```Python
>>> print "food is very nice" #eat me

food is very nice

(a normal output, without the smutty comment,
thankyou very much)

>>># print "food is very nice"

(nothing happens, because the code was after a comment)

>>> print "food is very nice" eat me

(you'll get a fairly harmless error message,
because you didn't put your comment after a hash)
```

---
#Η επανάληψη 'while'

```
while {condition that the loop continues}:
    {what to do in the loop}
    {have it indented, usually four spaces}
{the code here is not looped}
{because it isn't indented}
```
---
#Η επανάληψη 'while'

Παράδειγμα

```Python
a = 0
while a < 5:
    a = a + 1
    print a
```

---
#Η επανάληψη 'while'

Αυτό σημαίνει:

- 'a' είναι ίσο με 0
- Όσο το 'a' είναι λιγότερο από 5, κάνε τα παρακάτω:
  - Μεγάλωσε το 'a' κατά μία μονάδα παραπάνω απόσο είναι.
  - Τύπωσε στην οθόνη την αξία του 'a'.

---
#Η επανάληψη 'while'
##Βήμα - Βήμα

```
Is 'a' less than 5? YES (its 0)
Make 'a' one larger (now 1)
print on-screen what 'a' is (1)

Is 'a' less than 5? YES (its 1)
Make 'a' one larger (now 2)
print on-screen what 'a' is (2)

[...]

Is 'a' less than 5? YES (its 4)
Make 'a' one larger (now 5)
print on-screen what 'a' is (5)

Is 'a' less than 5? NO (its 5, therefore isn't less than 10)
Don't do the loop
There's no code left to do, so the program ends
```

---
#Η επανάληψη 'while'

```
while {condition that the loop continues}:
    {what to do in the loop}
    {have it indented, usually four spaces}
{the code here is not looped}
{because it isn't indented}
```
---
#Conditions

```python
while {conditions to be met}:

```

`{conditions to be met}` εννοούμε μία συνθήκη που είναι Αληθής (__TRUE__) ή Ψευδής (__FALSE__).

Δηλαδή η συνθήκη μας έχει μόνο δύο καταστάσεις και αυτό τη χαρακτηρίζει _Διαδική_ ή _Boolean_.

---
#Conditions
##Boolean

```
Expression 	Function

<           less than
<=          less that or equal to
>           greater than
>=	        greater than or equal to
!=	        not equal to
<>	        not equal to (alternate)
==	        equal to
```

---
#Statements
##if statement

```
if {conditions to be met}:
    {do this}
```

Παράδειγμα:

```Python
y = 1
if y == 1:
    print "y still equals 1, I was just checking"
```

---
#Statements
##if statement

Ακόμη ένα

```Python
print "We will show the even numbers up to 20"
n = 1
while n <= 20:
    if n % 2 == 0:
        print n
    n = n + 1
print "there, done."
```

---
#Statements
##else statement

```Python
a = 1
if a > 5:
    print "This shouldn't happen."
else:
    print "This should happen."
```

---
#Statements
##elif statement

```Python
z = 4
if z > 70:
    print "Something is very wrong"
elif z < 7:
    print "This is normal"
```

---
#Statements
##else & elif statement

```Python
if {conditions}:
    {run this code}
elif {conditions}:
    {run this code}
elif {conditions}:
    {run this code}
else:
    {run this code}
```

---
#Statements
##else & elif statement

Μπορείτε να έχετε όσα `elif` θέλετε. Από κανένα μέχρι τα πρωταθλήματα του Ολυμπιακού.

Μπορείτε να έχετε το πολύ ένα `else` και αυτό μετά από όλα τα άλλα `if` και `elif`.

---
#Indentation

```Python
a = 10
while a > 0:
    print a
    if a > 5:
        print "Big number!"
    elif a % 2 != 0:
        print "This is an odd number"
        print "It isn't greater than five, either"
    else:
        print "this number isn't greater than 5"
        print "nor is it odd"
        print "feeling special?"
    a = a - 1
    print "we just made 'a' one less than what it was!"
    print "and unless a is not greater than 0, we'll do the loop again."
print "well, it seems as if 'a' is now no bigger than 0!"
print "the loop is now over, and without furthur adue, so is this program!"
```

---
#Indentation

Όπως βλέπουμε δεν υπάρχουν παρενθέσεις.

Έχουμε κενά και ':' για να διαχωρίσουμε τι είναι μέσα στα statements και στις επαναλήψεις.

Αυτό είναι καλό και κακό ταυτόχρονα.

Σε κάθε περίπτωση ο προτεινόμενος τρόπος είναι να χρησιμοποιούμε 4 κενά ή το πλήκτρο `Tab`.

---
#Λίστες

```Python
>>> Avengers = ['Iron Man','Hulk','Hawkeye',\
'Thor','Black Widow','Captain America']
>>> print Avengers[2]
'Hawkeye'
```

---
#Λίστες

Ακούγεται ότι ο Spiderman θα είναι μέσα.

```Python
>>> Avengers = ['Iron Man','Hulk','Hawkeye',\
'Thor','Black Widow','Captain America']
>>> Avengers.append('Spiderman')
>>> print Avengers
['Iron Man','Hulk','Hawkeye','Thor',\
'Black Widow','Captain America','Spiderman']
```

---
#Λίστες

Ή και όχι.

```Python
>>> Avengers = ['Iron Man','Hulk','Hawkeye','Thor',\
'Black Widow','Captain America','Spiderman']
>>> del Avengers[-1]
>>> print Avengers
['Iron Man','Hulk','Hawkeye','Thor',\
'Black Widow','Captain America']
```

---
#Λεξικά

Ίσως το πιο σημαντικό στοιχείο της Python.

Μας επιτρέπει να αποθηκεύουμε και να διαχειριζόμαστε μοναδικά ζευγάρια δεδομένων με μία μορφή που λέγεται `key - value pairs`.

---
#Λεξικά

```Python
# Το ορίζουμε αυτό.
>>> Superheros = {}
>>> Superheros['Batman'] = 'Bruce Wayne'
>>> Superheros['Superman'] = 'Clark Kent'
>>> Superheros['Green Lantern'] = 'Hal Jordan'
>>> print (Superheros['Batman'])
Bruce Wayne
```

---
#Λεξικά

Μπορούμε να βάλουμε τα κλειδιά και τις τιμές σε λίστες.

```Python
>>> heros = Superheros.keys()
>>> identities = Superheros.values()
>>> print heros
['Batman', 'Superman', 'Green Lantern']
```

---
#Λεξικά

Τα λεξικά δεν έχουν κάποια σειρά. Το σύστημα τα προσπελάνει σε τυχαία σειρα.

Μπορούμε όμως να ταξινομίσουμε τις λίστες των κλειδιών και των τιμών.

```Python
>>> heros.sort()
>>> print heros
['Batman', 'Green Lantern', 'Superman']
```

---
#Λεξικά

Μπορούμε επίσης να ξέρουμε εύκολα πόσα στοιχεία έχει μέσα το λεξικό μας

```Python
>>> len(Superheros)
```

---
#Λεξικά

Το κλειδί πάντα είναι `String`.

Η τιμή όμως μπορεί να είναι οτιδήποτε. Όπως ολόκληρα λεξικά.

```Python
>>> players = {}
>>> players['Olympiakos'] = {}
>>> players['Olympiakos']['Kostas Giannoulis'] = 20
>>> players['Panathinaikos'] = {}
>>> players['Panathinaikos']['Panagiotis Spyropoulos'] = 2
>>> print players
{'Panathinaikos': {'Panagiotis Spyropoulos': 2}, 'Olympiakos': {'Kostas Giannoulis': 20}}
```

---
