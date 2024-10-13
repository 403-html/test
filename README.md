# TypeScript Recruitment Task

This is a repo for a recruitment task in TypeScript.

1. What this project is about?
This project is designed to assess your understanding of TypeScript concepts such as classes, interfaces, inheritance, access modifiers, and asynchronous operations.  You will implement a transaction system with basic validation.
2. How to run the project?
   1. What will happen when you run `npm run start` right away after cloning the project?
3. Implement abstract class "Transaction" where you'll store information about transaction (provided on init – amount, name, id). Also it'll by default have status "isProcessed" set to false.
   1. All of provided values should be `protected`.
   2. Explain the difference between `protected` and `private` in your own words.
   3. Implement a way for the user to get access to the `id` of the transaction. Let's assume that it'll return a string like "Transaction ID: 123, on amount: 1000".
   4. Implement a method for the user to "process" the transaction, which will set the status to true and print the message "Transaction ID: 123, on amount: 1000 has been processed".
4. Implement interface "CardTransaction" with a method "validate" which will return a boolean value in a Promise.
   1. Explain in your own words what an Interface is.
   2. Explain in your own words what a Promise is.
5. Implement class "CardTransaction" which will extend "Transaction" and implement "TransactionInterface". It should return `true` if the amount is greater than 0 and is not yet processed, and `false` otherwise. If the amount is less than or equal to zero, throw an error with a descriptive message.
6. In "main.ts" create an instance of "CardTransaction" and call the "validate" method on it. Processing should pass. Print the result to the console. Handle any potential errors during validation (even if in test run you'll not encounter any).
7. Run project, use successful transaction init data (amount > 0, id = 1, name = "Some transaction") and check if the transaction has been processed successfully.