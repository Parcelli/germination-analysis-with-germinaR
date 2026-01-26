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
* `Data/` → raw input data
* `Scripts/` → R scripts
* `Results/` → output tables
* `Figures/` → plots and figures

#### Create folders

1. In Files/plots/help pane in RStudio, click **New Folder**
2. Enter folder name 
3. Click Ok. Repeat this steps till you have all the folders created as below


<img width="984" height="569" alt="rproject_folder" src="https://github.com/user-attachments/assets/999f43a7-aae5-402f-9e51-0d1d294c0c98" />


