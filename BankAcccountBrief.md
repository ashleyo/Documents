# Bank Accounts - Brief

## Task Zero
Implement code representing bank accounts. The following objects/behaviours are required.

+  **Customer** who are identified by **Name** and may also have other properties
+ **Account** which will have a customer owner, **AccountHolder**,  and will be identified by an **AccountNumber**. There will be  **Deposit()** and **Withdraw()** methods and it will correctly maintain a **Balance** property.

+ A mechanism that allows all accounts, their owners and their balances to be listed 
*Hint: a collection class containing all accounts created?*

> You may freely use this [code](https://pastebin.com/6KHMr1PJ) if you wish,  to assist with logging output in order to check that things are working correctly. There is/will be also a suggestion as to how you might handle account numbers.

## Task One

+ Add a **CurrentAccount** which has the features above and a new property **OverdraftLimit**. This type of account will allow a negative balance until the Overdraft Limit is reached at which point no more withdrawals are possible. 
+ Prevent vanilla 'Accounts' from being created
*Hint: There is more than one way to do this. Eg abstract classes can not be instantiated; if a constructor is protected it is only accessible to derived classes; ... *


## Task Two

Now add a **Savings Account**. This type of account may not be overdrawn. The 'show all accounts' mechanism also needs to identify the type of account.

## Task Three
Now add a **PremiumSavingsAccount** This type of account also has a PayInterest() method that will add interest to the balance *if* the balance is above a **Threshold** amount, this last is to be implemented as a static property of the class (ie should be the same for all accounts of this type).

'Show all accounts' still needs to be working.

## Task Four

Change your implementation so that all accounts may have more than one account holder. It is permissable for the 'show all accounts' mechanism to mention only the first **AccountHolder**

### Questions ...

1. How many times did you change your implementation?
2. Did you use i) concrete classes + inheritance ii) abstract classes + concrete classes + inheritance iii) interfaces? What made your decision for you?
3. What woul you do differently if you were doing it again?
4. Suppose the bank now wanted a PremiumXtraAccount that combined features of a **Current Account** and a **Savings Account** in that it had an overdraft facility but also paid interest on positive balances above a threshold. How woul you implement that? You cannot inherit from multiple classes in C# and neither can you use 

### Extension

Read [this article](https://www.thoughtworks.com/insights/blog/composition-vs-inheritance-how-choose). Write down all the questions it raises in your mind. (There should be a lot! This is advanced material  written for an experienced audience). Discuss these questions with your colleagues and then with your tutor.
> Written with [StackEdit](https://stackedit.io/).

