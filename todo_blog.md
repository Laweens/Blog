
In class were currently working on a todo list that simply tracks items in a list and removes or adds items to the list depending on the users choice. 

First thing I did was i made a list "todos" to store everything, the rest of my code also revolves around the one list. 
``` pythonn
todos = [] 
```

I put an input to ask the user to add or remove from the list and I assigned it to the variable "todosadd"

``` python
todosadd = input("Do you wish to add or remove something from your list? ") 
```

All this code does is it gives the user the ability to type in with their keyboard whether they want to add or remove.
After the input i struggled for a while on my syntax, indentation and logic in my for loop, basically everything important.

After alot of racking my brain and thinking i finished the first part of my for loop but it still had alot of errors in the first few versions and eventually ended up with this. 

``` python

if todosadd == ("add"):
        print("")
        ADD = input ("what do you want to add ")
        print("--------------------------------------------------------")
        todos.append(ADD)
```
The code is the Addition portion of the loop that makes a new input and appends whatever you input into the list which i figured out fairly quickly and was the easiest portion on the todo list.

``` python
elif todosadd == ("remove"):
        print("")
        if len(todos) == 0:
            print("ERROR")
            print("")
            continue
        REMOVE = int(input("What would you like to remove? "))
        print("--------------------------------------------------------")
        print("")
        del todos[REMOVE - 1]
```

    The removing of items in the list was far more difficult than adding and took me a long time to fix and finalize, but it was also the last part of the TODO list. I had to search for the len function since we never used it or learned about it in class. Len keeps track of however long the list is and i use it in the code to not get an error if the user has nothing to remove.

    I used an elif to tell the computer the other option is to remove. Then i made a new variable for removing and made it an int since were removing based off the index. After that we just remove whatever the user picked from the list. THE END.

