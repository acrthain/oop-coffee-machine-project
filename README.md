# OOP Coffee Machine

A command-line coffee machine simulation built to practise object-oriented programming in Python.

## What it does

The program simulates a coffee machine that can serve **latte**, **espresso**, and **cappuccino**. It:

- Checks whether there are enough resources (water, milk, coffee) to make the selected drink
- Processes coin payments (quarters, dimes, nickels, pennies) and calculates change
- Refunds the customer if not enough money is inserted
- Tracks and reports total profit and remaining resources on request
- Can be turned off via a simple command

## How it works

The project is split into four modules, each with a single responsibility:

- **`main.py`** — runs the main program loop, handling user input and coordinating the other classes
- **`menu.py`** — defines `MenuItem` and `Menu` classes, representing the available drinks and their ingredients/cost
- **`coffee_maker.py`** — defines the `CoffeeMaker` class, which tracks resources and checks whether an order can be fulfilled
- **`money_machine.py`** — defines the `MoneyMachine` class, which handles coin processing, payment validation, and profit tracking

## Tech used

- Python 3
- Object-oriented design (encapsulation, single-responsibility classes)

## What I'd improve next

- Add input validation to handle non-numeric or negative coin entries gracefully
- Persist resource/profit data between runs
- Add unit tests for `is_resource_sufficient()` and `make_payment()`

## Background

Built as part of a 100 Days of Code Python bootcamp, while working toward a software engineering internship.
