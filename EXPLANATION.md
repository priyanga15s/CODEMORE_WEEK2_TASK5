# Explanation of Java Concepts Used

## Objective

This program demonstrates the concept of **Encapsulation** by creating a `BankAccount` class with private attributes and public getter and setter methods. It also validates the balance to prevent negative values.

---

# 1. Class

A class is a blueprint for creating objects.

```java
class BankAccount
```

The `BankAccount` class contains:

- Private attributes
- Constructor
- Getter methods
- Setter method

---

# 2. Encapsulation

Encapsulation is the process of wrapping data and methods into a single unit (class) and restricting direct access to the data.

Example:

```java
private String accountNumber;
private double balance;
```

The variables are declared as `private`, so they cannot be accessed directly outside the class.

---

# 3. Data Hiding

Data hiding protects an object's data from unauthorized access.

The `balance` can only be accessed or modified through public methods.

```java
private double balance;
```

---

# 4. Constructor

The constructor initializes the object when it is created.

```java
public BankAccount(String accountNumber, double balance)
```

It also checks that the initial balance is not negative.

---

# 5. Getter Methods

Getter methods return the value of private variables.

Example:

```java
public String getAccountNumber()
```

```java
public double getBalance()
```

These methods allow safe access to private data.

---

# 6. Setter Method

The setter method updates the balance after validating the input.

```java
public void setBalance(double balance)
```

Validation:

```java
if(balance >= 0)
```

If the balance is negative, an error message is displayed and the previous balance remains unchanged.

---

# 7. Validation

The program prevents invalid data.

Example:

```java
if(balance >= 0)
```

This ensures that the account balance is never negative.

---

# 8. Scanner Class

The `Scanner` class is used to read user input.

```java
Scanner sc = new Scanner(System.in);
```

Methods used:

- `nextLine()`
- `nextDouble()`

---

# 9. Objects

An object is created from the `BankAccount` class.

```java
BankAccount account = new BankAccount(accountNumber, balance);
```

The object stores account details and provides controlled access through methods.

---

# 10. Closing the Scanner

```java
sc.close();
```

This releases system resources after input is complete.

---

# Program Flow

1. Create the `BankAccount` class.
2. Declare `accountNumber` and `balance` as private.
3. Create a constructor to initialize the object.
4. Implement getter methods for account number and balance.
5. Implement a setter method with validation.
6. Read account details from the user.
7. Create a `BankAccount` object.
8. Display account details.
9. Update the balance using the setter.
10. Display the updated account details.
11. Close the `Scanner`.

---

# Java Concepts Covered

- Classes
- Objects
- Encapsulation
- Data Hiding
- Private Variables
- Getter Methods
- Setter Methods
- Constructors
- Validation
- Scanner Class
- User Input
- Output Statements
- Resource Management (`sc.close()`)
