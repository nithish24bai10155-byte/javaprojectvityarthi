# 💰 Student Expense Tracker

> A command-line Java application to help students monitor spending, set budgets, and gain insights into their financial habits.

**Author:** P NITHISH  
**Registration Number:** 24BAI10155  
**Course:** Programming in Java  

---

## 📌 Problem Statement

Students frequently lose track of daily expenditures — food, transport, stationery, entertainment — and realize at month-end they've overspent with no idea where the money went. There was no lightweight, offline, privacy-first tool that a student could run on any machine without internet or an account.

This project solves that by providing a simple terminal-based expense tracker built entirely in Java.

---

## ✨ Features

| Feature | Description |
|---|---|
| ➕ Add Expense | Record title, amount, category, date, and notes |
| 📋 View Expenses | Filter by this month, a specific month, category, or all-time |
| ✏️ Edit Expense | Modify any field of an existing record |
| 🗑️ Delete Expense | Remove a record by its unique ID |
| 🔍 Search | Keyword search across title and notes |
| 📊 Analytics | Category breakdown, monthly trend bar chart in terminal |
| 💼 Budget Manager | Set monthly and per-category spending limits with warnings |
| 📄 Export Report | Generate a formatted `.txt` monthly report |
| 💾 Persistence | All data saved locally as CSV — no database required |

---

## 🗂️ Project Structure

```
StudentExpenseTracker/
├── src/main/java/com/expensetracker/
│   ├── Main.java                    ← Entry point
│   ├── model/
│   │   ├── Expense.java             ← Expense entity (with CSV serialization)
│   │   └── Budget.java              ← Budget configuration model
│   ├── service/
│   │   └── ExpenseService.java      ← Business logic, analytics, filtering
│   ├── ui/
│   │   └── ConsoleUI.java           ← All terminal menus and user interaction
│   └── util/
│       ├── FileUtil.java            ← CSV read/write, report export
│       └── Validator.java           ← Input validation helpers
├── data/                            ← Auto-created; stores expenses.csv, budget.csv
├── README.md
└── ProjectReport.docx
```

---

## ⚙️ Setup & Run

### Prerequisites

- **Java 11 or higher** installed (`java -version` to check)
- No additional libraries required — pure Java standard library

### Compile

```bash
# From the project root directory
find src -name "*.java" > sources.txt
javac -d out @sources.txt
```

### Run

```bash
java -cp out com.expensetracker.Main
```

### Quick One-Liner (Linux/macOS)

```bash
find src -name "*.java" | xargs javac -d out && java -cp out com.expensetracker.Main
```

---

## 🚀 Usage Guide

When you launch the app you'll see the main menu:

```
╔══════════════════════════════════════════════╗
║     STUDENT EXPENSE TRACKER  v1.0           ║
║     P NITHISH  |  24BAI10155                ║
╚══════════════════════════════════════════════╝

  ┌──────────────────────────────────────────┐
  │  This Month: ₹1250.00 / ₹5000.00        │
  ├──────────────────────────────────────────┤
  │  1. Add Expense                          │
  │  2. View Expenses                        │
  │  3. Delete Expense                       │
  │  4. Edit Expense                         │
  │  5. Search Expenses                      │
  │  6. Analytics & Summary                  │
  │  7. Manage Budget                        │
  │  8. Export Monthly Report                │
  │  0. Exit                                 │
  └──────────────────────────────────────────┘
```

### Adding an Expense

```
Title: College Canteen Lunch
Amount (₹): 85
Select Category:
  1. FOOD  2. TRANSPORT  3. EDUCATION ...
Choice: 1
Date (YYYY-MM-DD, blank = today): [Enter]
Note (optional): Veg thali
✔ Expense added! ID: A3F7C921
```

### Viewing Analytics

The analytics view shows a terminal bar chart:

```
FOOD           ₹  2150.00   43.0%  ██████████
TRANSPORT      ₹  1200.00   24.0%  ██████
EDUCATION      ₹   850.00   17.0%  ████
ENTERTAINMENT  ₹   500.00   10.0%  ██
OTHER          ₹   300.00    6.0%  █
```

---

## 💾 Data Storage

All data is stored in the `data/` folder as plain CSV files:

- `data/expenses.csv` — All expense records
- `data/budget.csv` — Your budget configuration
- `data/report_YYYY_MM.txt` — Exported reports

This means your data is always yours — no cloud, no account, no internet needed.

---

## 🧪 Java Concepts Applied

- **OOP**: Classes, encapsulation, enums, constructors
- **Collections**: `ArrayList`, `HashMap`, `EnumMap`, `Stream API`
- **File I/O**: `BufferedReader`, `BufferedWriter`, `Files`, `Paths`
- **Exception Handling**: Try-catch, custom error messages
- **Java Time API**: `LocalDate`, `Month`, `DateTimeFormatter`
- **Lambdas & Streams**: Filtering, sorting, mapping, aggregation
- **Scanner**: Console input handling

---

## 📄 License

This project was created as a BYOP capstone for the Programming in Java course at VIT.
