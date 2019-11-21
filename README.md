# UniDaysChallenge
This is a C#  implementation of the UniDays code challenge. The program comes with a intuitive graphical user interface, built with Windows Forms to facilitate
testing. It should be run on any device with a Windows O.S. installed. A version of Visual Studio is required to run the code in Debug mode. The executable is located in the bin>Debug folder.
User Manual:
Plus and Minus Buttons - Use those to add and remove items from your shopping basket. 
Calculate Price - Use this button to calculate the total price of your order.
Start Over- Use this to re-load the page. All previous basket entries are discarded.


Approach:
All important functionality is captured in the Program.cs file.  I created the UnidaysDiscountChallenge class,
following the challenge overview as a software specification document. I created a class called Item to hold items' information. (Type/Price)
Methods within this class were used to set the item price in accordance to its type and provide other classes with access to the item's price.
The shopping basket was essentially a list of type Item. All of the methods withing the UnidaysDiscountChallenge class operated
on this list. To add/remove items from the basket, I implemented two methods, each taking a parameter of type Item and either 
added it or removed it from the list. The pricing rules were all implemented within the CalculatePrice method in the form of a sequence 
of if statements.On call, CalculatePrice returned the total price of the order, excluding the delivery charge. 
An additional method  called CalculateTotalPrice was added to calculate and return the overall total. 
