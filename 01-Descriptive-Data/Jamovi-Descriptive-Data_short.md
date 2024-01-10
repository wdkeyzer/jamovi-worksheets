---
title: 'Jamovi Basics & Descriptive Data'
abstract: |
    By the end of this worksheet, you will have an appreciation of the following Jamovi tools and functions:

    - Navigating and using the Jamovi environment 
    - Exploring and Creating Variables and Cases 
    - Descriptive Data 
    - Simple Graphs and Boxplots 
    - Parametric Testing

    ::: Questions
    As you work through this worksheet, there will be **learning checks** (numbered Q1, Q2, etc.) that ask you questions about what has just been covered. These questions are not submitted for assessment, they are just to help you fully learn how to use Jamovi. Answers to all the questions are provided at the end of this worksheet for you to check if you were correct and you can click the question numbers to jump to that answer.
    :::
---

\wordtoc

# Getting familiar with Jamovi

In this section, we will mostly just be getting used to how to use Jamovi, and how to set up our data.

## Installing Jamovi on your own computer

As Jamovi is a free and open-source application, you can easily install it on your own computer. Download the Jamovi installer for your system from:

[https://www.jamovi.org/download.html](https://www.jamovi.org/download.html)

If given the option, choose the '**Solid**' version. Once the installer is downloaded, double-click on it to install Jamovi to your computer. For a full walk-through and instructions on how to install Jamovi, see section 1 of the **Jamovi user-guide** here:

‌[https://www.jamovi.org/user-manual.html](https://www.jamovi.org/user-manual.html)

Jamovi is just a regular application installation for Windows and Mac, but Jamovi is also available for Linux and Chromebooks with some extra steps (see the user-guide link above for more detail). If for some reason you cannot install Jamovi on your computer, you can use an online version of Jamovi here:

[https://cloud.jamovi.org/](https://cloud.jamovi.org/)

::: Aside

Be aware that the online version of Jamovi is just a demo version, and may not always be reliably available. It is **strongly suggested** that you install Jamovi on your own computer if at all possible.

:::

## Help with Jamovi

Jamovi has a lot of resources online to help you use it! As well as the user-guide linked above, you can find a number of useful further guides at the Jamovi community resources page here:

[https://www.jamovi.org/community.html](https://www.jamovi.org/community.html)

In particular, there is a YouTube playlist of useful Jamovi video guides ([click here](https://bit.ly/jamovi-youtube)) and a full statistics textbook using Jamovi ([click here](https://www.learnstatswithjamovi.com/)) linked from the community resources page that might be useful if you need help outside of a tutorial, or want to know even more detail about stats with Jamovi.

## Download the data files

Download **all** the Jamovi data files from [GitHub](https://github.com/jmablog/jamovi-worksheets) and save them somewhere you can easily access them.

Jamovi uses the '.omv' file extension, which is a custom file format. Unlike other file formats, you might not be able to double-click these as a shortcut to open them in Jamovi - don't worry, you just need to open Jamovi first, then open them from within Jamovi.

## First look at Jamovi

After installing, open up the Jamovi application. You should see a blank Jamovi workspace:

![](_imgs/01-01.png)

The workspace in Jamovi is divided into a few sections.

- The large grid-like area on the left (that looks like Excel) is the **Spreadsheet**. This is where your data goes!
- The blank area on the right is the **Results Viewer**. This is like a blank sheet of paper where Jamovi prints out the results of any tests you run. You'll see how this works soon.
- At the top is the **Menu**. This has a few options - **Data**, **Analyses**, and **Edit**. We will mostly be using Data and Analyses. When you click any of these options, the **ribbon** area directly underneath changes to show you the things you can do with each option - in the screenshot above, we have **Analyses** selected, so the ribbon is showing us all the various Analyses tests we can run.

The menu also has three stacked white lines in the far left corner - this opens the **File** menu. Click it now, then click **Open**, then **Browse** and navigate to the place you saved all the data files from Weblearn:

![](_imgs/01-02.png)

Open the **Body Compsition.omv** file.

You should see data now in the Spreadsheet view. If you want to see more of the data, you can resize the Spreadsheet and Results Viewer by clicking and dragging the thick grey line in the middle of the screen.

![](_imgs/01-03.png)

## Cases and variables

In Jamovi, each **column** represents a **variable**, similar to Excel, and each **row** represents a **case**. In Excel, we had to create a dummy Participant ID column as our case identifier. This is the same in Jamovi, which has been named 'PartID' in this file.

::: Questions
[Q1]{}. How many columns of data are there?

[Q2]{}. How many rows of data are there?

[Q3]{}. Why bother with a Participant ID when there is a record number?

[Q4]{}. Why do we need a Participant ID at all? Why not just use the participant's name?

:::

Pay attention to the PartID column - note that some IDs are missing, so the row number does not always match the PartID.

I want you to add one further case to this data sheet, so just type in the following numbers at the bottom of the sheet. You can type directly into each cell (similar to Excel).

- PartID: 53
- Age: 21
- Gender: 2
- Course: [Leave blank]
- Weight: 41.0
- Height: 160.0
- BIA1: 18.8
- BIA2: 18.8
- FitPercept:     [Leave blank]

### Variables setup

So far this sheet is behaving much like Excel in what we can enter. However unlike Excel, Jamovi allows us to enter more information about  what is contained in each of our variables (the spreadsheet columns). This is known as **metadata**. To edit this, click **Data**, then **Setup** (the icon that looks like a gear on top of a mini-spreadsheet). You will get an extra menu open at the top of the Jamovi screen:

![](_imgs/01-04.png)

You can see the name of the variable we are editing at the top, in large text. This is the variable **Label**. Click on any cell in another column to change to that variable - see how the text at the top of the variable setup menu changes.

Directly underneath the large Label area is another text box - this is the **Description** area, where you can add a little extra text to make it clearer what is contained in our variable. Click on the PartID column and notice how it says 'Participant ID' now - this is the full name of the variable, rather than the shorter 'PartID' label.

::: Aside

Why do we use separate labels and descriptions? When you're working with a variable, sometimes it can be annoying to type in the full name over and over again - 'PartID' is a lot quicker to type than 'Participant ID'. But, when we want to see our results, we want the full description of the variable to make it easier and clearer to see what our results are referring to.

:::

I now want you to change a couple of variable properties:

- You can see that most of our variables have a Name and Description, but two are missing. For the column **Age** enter the description 'Age (years)' and for the **Gender** column enter the description 'Gender'.

