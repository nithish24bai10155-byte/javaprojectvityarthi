# Student Expense Tracker

A simple Java app to help Student Expense Tracker users stay in control of their money. Without needing the internet accounts or complicated tools.

**Created by:** P Nithish

**Reg No:** 24BAI10155

**Course:** Programming in Java

---

## Why Student Expense Tracker Exists

Let us be honest. Most students do not track their spending.

You grab snacks, book rides buy notes maybe go out with friends… and suddenly your money is gone.

At the end of the month you are left wondering:

“Where did all my money go?"

Student Expense Tracker solves that problem.

Of using complex apps or relying on internet-based tools this is a lightweight offline expense tracker that runs directly in your terminal. Fast, private and distraction-free.

Student Expense Tracker is a solution to a common problem.

---

## What You Can Do With Student Expense Tracker

Think of Student Expense Tracker as your money assistant.

### Track Everything With Student Expense Tracker

* Add expenses with title, amount, category and notes

* Automatically assigns an ID to each entry

### Find Anything Quickly With Student Expense Tracker

* Search by keywords

* Filter by month or category

* View all-time or specific data

### Stay Flexible With Student Expense Tracker

* Edit any expense anytime

* Delete records you no longer need

### Understand Your Spending With Student Expense Tracker

* See category- breakdowns

* Visual terminal bar charts

* Monthly spending trends

### Control Your Budget With Student Expense Tracker

* Set limits

* Add category-wise budgets

* Get warnings before overspending

### Export Reports With Student Expense Tracker

* Generate monthly reports

* Great for reviewing or submitting

### Student Expense Tracker Is 100% Offline & Private

* No login

* No cloud

* No tracking

* Your data is your control

---

## Project Structure

```

StudentExpenseTracker/

├── Main.java              → Starts the Student Expense Tracker app

├── model/                → Data classes

├── service/              → Core logic & calculations

├──                   → Terminal interface

├── util/                 → File handling & validation

├── data/                 → Stores your CSV files

```

Everything is cleanly separated so it is easy to understand and extend.

---

## How to Run Student Expense Tracker

### Requirements

* Java 11. Higher

* That is it. No external libraries needed

### Compile & Run Student Expense Tracker

```bash

find src -name "*.java" > sources.txt

javac -d out @sources.txt

java -cp out com.expensetracker.Main

```

Or simply:

```bash

find src -name "*.java" | xargs javac -d out && java -cp out com.expensetracker.

```

---

## What Student Expense Tracker Looks Like

When you start the Student Expense Tracker app you will see a clean menu like this:

```

STUDENT EXPENSE TRACKER

This Month: ₹1250 / ₹5000

1. Add Expense

2. View Expenses

3. Delete Expense

4. Edit Expense

5. Search

6. Analytics

7. Budget

8. Export Report

0. Exit

```

Student Expense Tracker is simple and fast.

---

## Example Insight From Student Expense Tracker

```

FOOD           ₹2150   ██████████

TRANSPORT      ₹1200   ██████

EDUCATION      ₹850    ████

```

You instantly know where your money is going with Student Expense Tracker.

---

## How Your Data Is Stored With Student Expense Tracker

Everything is saved locally in CSV files:

* expenses.csv → All your records

* budget.csv → Budget settings

* report_YYYY_MM.txt → reports

No database.

No setup.

No risk of losing control with Student Expense Tracker.

---

## What I Learned From Student Expense Tracker

This project helped me apply core Java concepts in a way:

* Object-Oriented Programming

* Collections & Streams

* File Handling

* Exception Handling

* Java Time API

* Clean code structuring

---

## Final Thoughts On Student Expense Tracker

This is not a project. It is something you can actually use daily.

If you are a student who wants to:

* stop overspending

* understand your habits

* stay organized

…Student Expense Tracker does that without overcomplicating things.

---

## License

Created as a capstone project for the Programming in Java course, at VIT.
