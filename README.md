AssociateProfitSplitter contract takes ETHs into contract and divides it evenly among 3 associate level employees, allowing fast and efficient payment. 

First thing is to initiate the contract, in this case it is AssociateProfitSplitter.

Then create 3 payable addresses.  Curly brackets incapsulate the code. 
Then initializing and definiing the public variables for employee_one, employee_two, and employee_three.

Next constructor function takes all three payable addresses and sets equal parameter values
(optional function that is executed upon contract creation)

Balance function gets the balance for this contract address sets in non negative integer and returns the contract address balance (Function -reuasable code that can used again and again wihtout typing over.) 

Deposit function  (.transfer means that certain amount will be transfered from ths address to someone else)
Allows for deposit in contact split among 3 employeess and equal amount is transferred to each employee.  The remaining balance (if any) is sent back to Human Resources.


In funciton external payable. Payable emplies that the contact is able to withdraw, receive or send money. 
Prevents from losing eths to a void, for catching ether sent to this address outside of the transfer


TieredProfitSplitter contract distributes different levels of ETHs to eployess as different levels 60-25-15
Initiate the contract and call the variables (different tier employees)

constructor initiates the set up of address of each employee

function balance returns balance of sender's address
deposit function calculates points by taking incoming payment and dividing it by 100 to determine percentage 
(used to store the amount to send each employee), amoun is multiplied by points to distribute by percentage with 
first for CEO- 60%, then for CTO -25%, and Bob- 15%

The remaider gets sent to the emplyee with the highest percentage (CEO) by subtracting total from msg.value (incoming payment) 