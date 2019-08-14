# Divide_the_shit_equally

## This light-weight command line applet allows you to calculate money stuffs easily.

Have you ever encountered such a situation:

You, Allen, Alex, and Lily had a fantastic day. However, you paid for the lunch, Allen paid for the Uber ride, Alex booked four movie tickets online for Avengers 5, and Lily transfered Allen 40 bucks mistakenly. <br>

You folks want to split the money evenly but it seems so freakingly involved to get a correct amount of money to whom each one should transfer. Probably even James, the guy who is super frigging good at maths, will also be stuck by this problem… for 30 seconds. <br>



### Don't worry

**Divide_the_shit_equally** comes to help.

<br>


# How do I install it?

## For programmers

1. open terminal (or your favorite command line tool)

2. run ``` $ git clone git@github.com:JamesSMF/divide_the_shit_equally.git ```

3. run 
```python money.py ```
inside the git directory diectly. (in python 2)



## For non-programmers

1. Prepare a mac, and make sure you have python 2 installed since this program is written in python 2. 

2. Click the green button "clone or download"




3. Click **Download ZIP**

4. Open **System Preference -> Security & Privacy**

5. Click the small lock and enter your password (Do I seem like a fraud…? Trust me tho lol.)

6. Click the small plus sign and select Downloads -> Divide_the_shit_equally-master -> Divide_the_shit_equally



### (There are 2 options for the next step)

**If you know how to use spotlight search:**

   Press command + \<space> and type "Divide_the_shit_equally" (without quotation marks) and press enter.

**else:**

   Open the Finder, and go to Downloads -> Divide_the_shit_equally-master. Click the Divide_the_shit_equally app to run it.


<br>


# Basic Usage

run

```bash
python money.py
```

to start the program.



*Note: there is no database for the program. So each time you run the program, all the previous datas are cleared.*



## New Event

Type "New event" or "new event" or simply "ne" to create a new event. <br>

Then, the program will prompt the user to enter people's names. You can split names by any character you like, but **not English letters**. <br>

After that, enter the event name. For example, "A Fabulous day". <br>

When you see

```bash
>>>
```

at the beginning of the line, you have successfully entered "event mode"



### Event Mode

#### Basic syntax

* \<person> trans \<person> \<amount of money> 
* \<person> pay \<amount of money>

Feel free to make those verbs gramatically correct, but please try not to change the basic structure of the syntax.<br>

Enter "q" or "Q" to quit event mode and go back to normal mode.



## Result

When you type "result" or "Result", the program will enter its calculation process and soon return the final result.<br>

The result is normally in this form:

\<name> {\<person>: \<amount of money>, \<person>: \<amount of money>, ... }

...



\<name> is the person who should transfer \<amount of money> to  \<person>.



## Q

Enter "Q" or "q" to exit the program cleanly.



<br>



# Version 1.2: File Mode

The newly added feather allows the user to input a file.

The basic syntax has not changed with some parts slightly different.

<br>

#### Here is an example file

```
Event: A fantanstic day in San Fransisco
People: Jack, Flora, Mely
   Jack paid 40 bucks for lunch
   Mely trans Jack 10 bucks
   Flora paid 20 dollars for Uber

Event: House rent
People: James, George, Johanna
   Johanna paid 3000 bucks for the rent
   James paid 200 for garbage disposal fee
   George trans James 30 bucks
   
result
```



Indentations and empty lines are not necessary but good for readibility.

Runnnig ``` python money.py <file name>``` will generate the result according to the content in the file.