# Background
menu.py is an ordering system from a food truck menu that keeps track of a customer's order and at end, prints everything on the order as well as the grand total. 

# Location of GIT repository
[https://github.com/mattledevs/python-challenge-1](https://github.com/mattledevs/python-challenge-1)

# Function of menu.py
A food menu will be printed for the customer. Customers will be able to place an order, which includes storing the customer's order and printing the receipt with the total price of all items ordered.

## Order System
An empty list is created for the customer's order in dictionary format.

After the sub-menu is printed, the customer is promped to enter their selection from the menu, saving it as a variable menu_selection.

Input validation is used to check if the customer input menu_selection is a number. If it isn't, an error message is printed.

If the user input is not in the menu_items keys, it will print an error. Otherwise, one of the following actions will be performed:

Get the item name from the menu_items dictionary and store it as a variable.

Ask the customer for the quantity of the menu item, using the item name variable in the question, and let them know that the quantity will default to 1 if their input is invalid. Save their answer as a variable called quantity.

Check that the customer input is a number. If it isn't, set the quantity to the value 1. If it is a number, convert the variable to an integer.

Append the customer's order to the order list in dictionary format with the following keys: "Item name", "Price", and "Quantity.

With each entry, the entire list of the customer's order will be printed remdinding the customer of what they ordered. 

Inside the continuous while loop that prompts the customer if they would like to keep ordering, a match case statement will check for y or n (upper or lowercase), and includes a default option if neither letter is entered by the customer.

## Order Receipt
Inside the loop of the customer order, the value of each key will be saved as their own variable: item_name, price, and quantity as well as adding to a grand total of the item number multipled by its quantity. 

This will all be printed out. 