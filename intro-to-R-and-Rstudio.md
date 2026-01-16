# Introduction to R and Rstudio

## What are R and Rstudio
R is a programming language widely used for statistics and data analysis in various fields.
R studio is a software interface that makes it easier to write R scripts and interact with the R software.

## Why use R ?
* **Reproducibility**

  R promotes reproducible research.  
  By writing your analysis as an R code you create a complete and transparent record of your analysis from data import to final results. This means that you or anyone else can reproduce the same results using the same data and script.Reproducibility is now a key requirement for most funders and journals.
    
* **Publlication quality plots**
  
  R has powerful visualization tools designed for creating high quality plots. Packages such a ggplot2 allow you to create clean, customizable and publication ready figures .

  
* **Less point and click**
  
  Unlike gaphical user interface (GUI) software, R does not depend on remembering which buttons to click or the order in which they were clicked.
  Instead your entire analysis is written as a script. To repeat or update the analysis , you simply run the script again ensuring consistency and reducing human error.
  
* **Strong and supportive Community**

  R has a large and supportive community. If you get stuck , help is widely available through platforms such as:
  - Stack Overflow
  - Rstudio community
  - Github
  - Blogs and tutorials
  This makes learning and troubleshooting much easier, especially for beginners.

## Installing R and R studio

To follow this tutorial, you need to install R and RStudio on your computer. Below are instructions on how to install R and Rstudio for windows.

**Step 1: Install R**

* Go to the Comprehensive R Archive Network (CRAN):
https://cran.r-project.org

* Click Download R for Windows

* Select base

* Click Download R x.x.x for Windows (choose the latest version)

* Open the downloaded file and follow the installation prompts (You can accept the default settings)

**Step 2: Install RStudio**

* Visit the RStudio website: https://posit.co/download/rstudio-desktop/

* Download RStudio Desktop (Free) for Windows

* Open the installer and follow the setup instructions


**Step 3: Verify the Installation**

Open RStudio

In the Console pane, type:

```
version

```
If R is correctly installed you will get information about the R version installed.

*💡 Helpful Tip for Beginners*

- Install R first before Rstudio. Rstudio will not work without R.
- You only need to install R once, but you may occassionally update it when a new versions are released.

## Navigating RStudio
When you open RStudio, you will see several panels (called panes) arranged in a default layout. Each pane has a specific purpose and helps you work efficiently in R.

In the default layout, RStudio has four panes:

<img width="960" height="540" alt="rstudio" src="https://github.com/user-attachments/assets/784558e9-2820-4d43-8bfe-aecfeb8667b6" />

## Working in R and RStudio

Before we begin the germination analysis, it’s important to understand a few basic concepts that will help you work efficiently and confidently in R and RStudio. This section introduces the essential building blocks you need — no prior programming experience required.

### Setting Up an R Project

An **R project** helps you keep all your files (data, scripts, and results) organized in one place.
Using projects also makes your work more **reproducible** and avoids problems with file paths.

### Create a New Project

1. In RStudio, click **File → New Project**
2. Choose **New Directory**
3. Select **New Project**
4. Give your project a name for now use **germination_analysis_R**. On the create project as a subdirectory of: Browse and select desired location to have your project ( we recommend desktop) for this tutorial. You can later move the folder to your desired location.
5. Click **Create Project**

RStudio will open a new session inside your project folder.

### Recommended Folder Structure

Inside your project, create the following folders:

```
project_folder/
├── data/
├── scripts/
├── results/
├── figures/
```

* `data/` → raw input data
* `scripts/` → R scripts
* `results/` → output tables
* `figures/` → plots and figures

---

## 🧾 Introduction to R Scripts

An **R script** is a text file where you write R code.

* Scripts allow you to **save**, **re-run**, and **share** your analysis
* They provide a complete record of your work

Create a new script:

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




