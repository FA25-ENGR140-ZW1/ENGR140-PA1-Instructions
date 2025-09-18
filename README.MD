# C++ Programming Assignment: Simple Banking System

## Objective
Create a C++ program that simulates basic banking operations using variables, arithmetic, and if-else statements.

## Requirements

### Part 1: Account Setup
Your program should prompt the user to enter:
- Account holder's name (string)
- Initial account balance (double)
- Account type: 1 for Checking, 2 for Savings (int)

### Part 2: Transaction Processing
Ask the user what operation they want to perform:
- 1: Make a deposit
- 2: Make a withdrawal  
- 3: Check balance
- 4: Calculate interest (savings accounts only)

### Part 3: Transaction Logic
Using if-else statements:
- **Deposit**: Add amount to balance, but reject negative amounts
- **Withdrawal**: 
  - Checking accounts: Allow overdraft up to $100 (charge $35 fee)
  - Savings accounts: Reject if insufficient funds
- **Interest**: Savings accounts earn 2.5% annual interest (calculate monthly)

### Part 4: Account Fees
Apply these rules with if-else statements:
- Checking accounts with balance below $500: $10 monthly fee
- All accounts: $25 fee for returned transactions

## Sample Output
```
=== SIMPLE BANKING SYSTEM ===
Enter account holder name: Sarah Johnson
Enter initial balance: $1250.00
Select account type (1-Checking, 2-Savings): 2

Current balance: $1250.00
Choose operation:
1. Deposit
2. Withdrawal
3. Check Balance
4. Calculate Interest
Enter choice: 2

Enter withdrawal amount: $300.00
Transaction successful!
New balance: $950.00
```

## Technical Requirements
- Use `int`, `double`, and `string` variables
- Implement nested if-else statements for different account types
- Use arithmetic operators for calculations
- Validate user input (no negative amounts, valid menu choices)
- Format currency output to 2 decimal places

## Concepts Covered
- Variable declarations and initialization
- User input with `cin`
- Arithmetic operations (`+`, `-`, `*`, `/`)
- Conditional statements (`if`, `else if`, `else`)
- Input validation
- Basic program flow control

## Bonus Challenges (Optional)
1. Keep track of number of transactions and apply fees accordingly
2. Add a "transfer between accounts" option
3. Implement a simple PIN verification system
4. Add transaction history display
5.  Savings accounts with more than 3 withdrawals: $5 per extra withdrawal

## Test Cases
Your program should handle:
- Valid deposits and withdrawals
- Overdraft attempts
- Invalid input (negative amounts, wrong menu choices)
- Interest calculations for savings accounts
- Fee applications based on account type and balance

## Submission Guidelines
- Save your file as `banking_system.cpp`
- Include comments explaining your logic
- Test with various scenarios to ensure robustness
- Make sure your program compiles and runs without errors

## Grading Criteria
- **Functionality (40%)**: Program works as specified
- **Code Quality (30%)**: Clean, readable code with appropriate comments
- **Input Validation (20%)**: Proper handling of invalid inputs
- **Testing (10%)**: Evidence of thorough testing with different scenarios
