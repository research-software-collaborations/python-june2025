# 009 - Vegetable Market

![Vegetable Market](../assets/vegetable-market.jpg)

You will now create a small program to simulate a vegetable market. We will build this up in step.

### Task 1:
  * First create a list of vegetables (and/or fruits, we will refer to both possibilities as "vegetables" below for simplicity)
  * Get the name of a vegetable as input from the keyboard/user. Check if it is in the list you have and print something to indicate that you do or do not.

### Task 2: 
  * If you have not already done so, make sure your code handles variations in letter case (both "peas" and "Peas" should match if that is in your vegetable list)
  * Now create a dictionary "inventory" whose keys are the names of the vegetables and whose values are random numbers between 0 and 6. This will be the number of that kind of vegetable that are available at your market stand.
  * Create a second dictionary "prices" whose keys are the names of the vegetables and who values are random numbers in [10,20,30,40,50,60,70,80,90,100]. This will be the price of one item of that type of vegetable.

### Task 3: 
  * Modify your code to take the name of a vegetable as input from the user. As before check if that vegetable is in your list. If it is, state the number available and the price. If the vegetable isn't available, print that it isn't.

### Task 4: 
  * Create a dict called bank with variables "wallet" and stand at the top of your program. Set "wallet" to 200 and "stand" to 0 initially. This will track the funds you have available to spend and the funds the stand has acquired.
  * Create an empty dict called "basket". This will track the items you have purchased (as keys) and how many of each type (as values).
  * Now some sort of loop around asking for input from the user. Allow the user to input one of a set of commands
    * "buy" - buys a vegetable and updates the bank, inventory, basket as needed. Add the obvious checks that you have enough money to buy an item, that the stand has the item in its inventory, etc.
    * "menu" - prints the list of available vegetables, their prices and the number available
    * "basket" - prints what you have purchased
    * "wallet" - tells you how much money you have
    * "stand" - tells you how much money the stand has.
    * "quit" - exits the program (with "Good Bye!")
