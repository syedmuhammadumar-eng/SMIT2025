# Functions Breakdowns (Define modules to work on) (According to Functionality)
# (Strategy => we will Create Project module by module)

- F1 creating an account,
- F2 depositing money,
- F3 withdrawing money,
- F4 checking the balance, 
- F5 printing a transaction statement, 

<!-- The system will be implemented using functions and basic data structures like lists and dictionaries -->
<!-- You will use a dictionary to store account details, including the balance and a list to track
transactions. Each action (deposit, withdrawal) will be represented as a separate function.  -->



# Steps:

# Step 1: Create an Account 

<!-- When a user opens an account, we will store their details in a dictionary. The dictionary will
contain: 
    The account holder’s name. 
    The balance (default is 0). 
    A list of transactions (which starts as empty).

Data structure: 
    account = { 
        "name": "John Doe",
        "balance": 0.0,
        "transactions": [] 
 -->


 <!-- 
 multiple accounts
 multiple users
 
 steps like 
 first ask do you have account or verify through account number yes or No
 if dont have account or invalid account number so give option to create account
 after succsuflly creating account show you are now onboard

 then provide select options like next, and exit
 all runs into a loop

 one loop > one function for handling account 

 data structure dicct
 account > user > user info with balance and transaction
  -->


# Step 2: Deposit Money 

<!-- The deposit function will add money to the user’s account balance. Each deposit will be
recorded as a transaction (deposit) in the transaction document via file read write to store
transactions permanently. 
    Function requirements: 
        The deposit amount must be positive. 
        Add the deposit amount to the current balance. 
        Record the deposit in the transaction in file 
 -->


# Step 3: Withdraw Money 

<!-- The withdraw function allows the user to withdraw money from the account. 
    Function requirements: 
        The withdrawal amount must be positive. 
        The user must have enough balance to withdraw the money. 
        If the withdrawal is successful, subtract the withdrawal amount from the balance and record the transaction. 
        If the balance is insufficient, print an error message. 
 -->

# Step 4: Check Balance 

<!-- The check_balance function simply returns the current balance from the dictionary. 
 -->

# Step 5: Print Statement 

<!-- The print_statement function will display all transactions made on the account (deposits and
withdrawals) and the balance after each transaction. -->

<!-- ==================================== Functional Breakdown ============================================ -->

# 1. Create Account
o This will initialize the account with a name, balance, and an empty transaction
list. 


# 2. Deposit Function
o Takes the current account and the amount to deposit as inputs.
o Updates the balance and records the deposit in the transaction list. 

# 3. Withdraw Function
o Takes the current account and the amount to withdraw.
o Checks if the balance is sufficient and updates the balance if the withdrawal is
successful.
o Records the withdrawal in the transaction list or prints an error message if the
withdrawal is not possible. 


# 4. Check Balance
o Simply returns the balance from the account. 


# 5. Print Statement
o Prints all transactions, showing the type of transaction (Deposit or Withdrawal)
and the balance after each transaction. 



<!-- ================================================  Additional Considerations   =================================================== -->

#  Error Handling:
You need to handle common errors such as:
o Attempting to deposit a negative amount.
o Trying to withdraw more money than the account balance.
o Printing an empty statement if no transactions have occurred. 


#  Edge Cases:
Test your functions with edge cases, such as:
o Depositing a negative value.
o Withdrawing more than the current balance.
o Ensuring the account balance cannot go negative. 

