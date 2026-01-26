## ntroduction to R Scripts

An **R script** is a text file where you write R code.

* Scripts allow you to **save**, **re-run**, and **share** your analysis
* They provide a complete record of your work

To Create a new script:

* **Mac:** `Shift + Cmd + N`
* **Windows/Linux:** `Shift + Ctrl + N`

### Comments

Comments are lines that R ignores. They are used to explain your code.

```r
# This is a comment
# Comments help explain what your code is doing
```

Good commenting makes your scripts easier to understand — for you and for others.

---

## 📦 Object Assignment

In R, results are stored as **objects**.

```r
germ_data <- read.csv("data/germination_data.csv")
```

* `<-` assigns a value to an object
* `germ_data` now stores your data in memory

You will see created objects appear in the **Environment pane**.

---

## 🔢 Basic Data Types

You don’t need to learn all data types to get started. The most common ones are:

* **Numeric** – numbers (e.g. germination counts)
* **Character** – text (e.g. treatment names)
* **Logical** – TRUE or FALSE
* **Data frame** – tables of data (most important)

Check the structure of your data:

```r
str(germ_data)
```

---

## 📦 Installing and Loading Packages

Packages extend R’s functionality.

### Installing Packages (once)

```r
install.packages("geminaR")
```

### Loading Packages (every session)

```r
library(geminaR)
```

📌 Important:

* Install a package **once**
* Load it **every time** you start a new R session

---

## ❓ Getting Help and Reading Documentation

R has built-in help files for all functions and packages.

To open a help page:

```r
?germination.metrics
```

Or:

```r
help(germination.metrics)
```

Help pages describe:

* What the function does
* Its arguments
* Example usage

Learning to read help files is a key skill for becoming independent in R.

---

## ⚠️ Understanding Error Messages

Errors are a normal part of learning R.

Common beginner errors include:

* Objects not found
* Misspelled function names
* Using the wrong data type

When you see an error:

1. Read the message carefully
2. Check object names and spelling
3. Make sure required packages are loaded

Errors are not failures — they are feedback.

---

## ✅ Key Takeaways

* Use **projects** to stay organized
* Extend R using **packages**
* Use **help files** to learn and troubleshoot

With these basics in place, you’re ready to start analyzing germination data using **germinaR**.
