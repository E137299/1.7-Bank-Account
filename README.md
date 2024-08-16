# 1.7 Bank Account

Notes: [print(), input(), variables, math and string operators](https://colab.research.google.com/drive/1JSrOECf5FeozLVAlGu7IDqGoR6bf3mR1?usp=drive_link)

<br></br>

**Objective:**  
Write a Python script that simulates a simple bank account where a user can perform a single transaction: deposit money, withdraw money, or check their balance. The script should ensure that the user cannot withdraw more money than is available in their account.

**Instructions:**  

**Step 1: Initial Setup**

1. Create a variable named `balance` and set it to `1000`. This variable will represent the user's bank account balance.

**Step 2: User Interaction**

2. Display the current balance and a menu that allows the user to choose between depositing money, withdrawing money, or checking their balance. The menu should look like this:
   ```
   Balance: 1000
   What would you like to do?
   1. Deposit
   2. Withdraw
   3. Check Balance
   ```
3. Prompt the user to select an option by entering a number (1-3).

**Step 3: Deposit Money**

4. If the user chooses to deposit money (option 1):
   - Prompt the user to enter the amount they wish to deposit.
   - Add the entered amount to the `balance`.
   - Print a message confirming the deposit and displaying the new balance.

**Step 4: Withdraw Money**

5. If the user chooses to withdraw money (option 2):
   - Prompt the user to enter the amount they wish to withdraw.
   - Before withdrawing, check if the `balance` is sufficient:
     - If the `balance` is sufficient, subtract the amount from the `balance`.
     - If the `balance` is not sufficient, print a message that the withdrawal cannot be completed due to insufficient funds.
   - Print a message confirming the withdrawal and displaying the new balance if the withdrawal was successful.

**Step 5: Check Balance**

6. If the user chooses to check their balance (option 3):
   - Print the current balance.

**Example**

Sample interaction with the program:
```
Balance: 1000
What would you like to do?
1. Deposit
2. Withdraw
3. Check Balance
Enter a number: 1
Enter the amount to deposit: 100
You have deposited $100. Your new balance is $1100.
```
or:
```
Balance: 1000
What would you like to do?
1. Deposit
2. Withdraw
3. Check Balance
Enter a number: 2
Enter the amount to withdraw: 50
You have withdrawn $50. Your new balance is $950.
```
or:
```
Balance: 1000
What would you like to do?
1. Deposit
2. Withdraw
3. Check Balance
Enter a number: 2
Enter the amount to withdraw: 1001
Error: Insufficient funds. You cannot overdraft your account.
```
or
```
What would you like to do?
1. Deposit
2. Withdraw
3. Check Balance
Enter a number: 3
Your current balance is $0.
```

