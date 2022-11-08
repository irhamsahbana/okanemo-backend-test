# Software engineer test - Type D: ATM - Retail Bank

## **Nature of the Game**

We want to understand the ideal would be a real-world problem with real scale, but that isn’t practical as it would take too much time. So instead, we have a dead-simple, high-school level problem that we want you to solve as though it was a real-world problem.

## **Rules of the Game**

Please complete the exercise using any programming language in PHP/Java/Javascript/Ruby/Python derivatives that you are most comfortable with. Your application must run and please include instruction manual for operation, If there are special cases or ambiguity, please take your own decision on how it should be handled and explain your decision. If you made any assumptions and/or deviations from the problem statement, please detail your reasoning.

You are allowed to use any library, but you should not use any library that outright solves the problem You should aim to implement to a level where you would be proud to have other engineers look and review your result. All parts of your submission will be assessed including but not limited to: Design choices (maintainability, legibility. Refactorability, extensibility) Implementation technique (including tests) Exception handling and special case handling.

## **Problem Statement**

You are asked to develop a Command Line Interface (CLI) to simulate an interaction of an ATM with a retail bank.

## Commands

- `login [name]` - Login as this customer and creates the customer if not exist
- `deposit [amount]` - Deposits this amount to the logged in customer
- `withdraw [amount]` - Withdraws this amount from the logged in customer
- `transfer [target] [amount]` - Transfers this amount from the logged in customer to the target customer
- `logout` - Logout of the current customer

## Example session

Your console output should contain at least the following output depending on the scenario and commands. But feel free to add extra output as you see fit.

```bash
$ login Alice

Hello, Alice!

Your balance is $0

$ deposit 100

Your balance is $100

$ logout

Goodbye, Alice!

$ login Bob

Hello, Bob!

Your balance is $0

$ deposit 80

Your balance is $80

$ transfer Alice 50

Transferred $50 to Alice

your balance is $30

$ transfer Alice 100

Transferred $30 to Alice

Your balance is $0

Owed $70 to Alice

$ deposit 30

Transferred $30 to Alice

Your balance is $0

Owed $40 to Alice

$ logout

Goodbye, Bob!

$ login Alice

Hello, Alice!

Your balance is $210

Owed $40 from Bob

$ transfer Bob 30

Your balance is $210

Owed $10 from Bob

$ logout

Goodbye, Alice!

$ login Bob

Hello, Bob!

Your balance is $0

Owed $10 to Alice

$ deposit 100

Transferred $10 to Alice

Your balance is $90

$ logout

Goodbye, Bob!
```
