# Automated_Fund_Portfolio_PnL

# Table of Content
### [Introduction](#introduction-1)
### [Assumptions](#assumptions-1)
### [Automated_Fund_Portfolio_PnL processflow diagram](#automated_fund_nav_calculation_processflow-diagram-1)
### [Steps to run the macro](#steps-to-run-the-macro-1)
### [Forward](#forward-1)

# Introduction
The purpose of [Portfolio_P&L.xlsm](https://github.com/Vanipreet/Automated_Fund_Portfolio_PnL/blob/master/Portfolio%20P%26L/Portfolio_P%26L.xlsm) is to create an automated process for the execution of Portfolio's / Fund's profit and loss analysis. There are multiple assumptions and pre-requisites that has been kept in place for the smooth execution of this macro.

# Assumptions
This macro is built with few assumptions in mind as listed below

1. For the macro to run, we need two external data inputs, pricing data and transactions data
2. The macro is prepared for the purpose of daily portfolio valuation and hence uses daily pricing data
3. Initial investment is assumed to be USD 800,000 
4. Macro and the data inputs are available under H:\Portfolio P&L directory, however as per the drive parition, this can be amended
5. Macro expects static input data. However with appropriate mapping, database can be also accurated utilized


# Automated_Fund_Portfolio_PnL processflow diagram
![alt text](https://github.com/Vanipreet/Automated_Fund_Portfolio_PnL/blob/master/ProcessFlow%20Diagram.png)

# Steps to run the macro

1. Download the zip file [Portfolio P&L](https://github.com/Vanipreet/Automated_Fund_Portfolio_PnL/tree/master/Portfolio%20P%26L) onto your preferred location and unzip the file there
2. Open "Portfolio_P&L.xlsm" workbook
3. Right click on macro button "Portfolio_PnL"
4. From the drop down options click on "Assign Macro"
5. Select "Portfolio_PnL" and click on "Edit" button
6. Under module 1, map the Pricing and Transactions file directory as per requirement
Please Note: All the mapping is required only on the Module 1
7. For test run, change the file name "Pricing_05082020.xlsx" to current Date, Month and Year in DDMMYYYY format. Save the file and close
8. Redo the Step 7 for "Transactions_05082020.xlsx" as well. 
9. Click on "Portfolio_PnL" macro button under Control sheet of "Portfolio_P&L.xlsm"

# Forward

This macro is a starting step for Portfolio P&L Analysis, utilizing some tweaks this can accurately fulfil Portfolio P&L Analysis requirement.

However the bigger picture is that instead of making this macro to work on a single fund, it can be accurately "Looped" for multiple funds.

If this macro is to run on windows system, "Task Scheduler" can be utilized to automatically update the input files at a precribed time from the source drive and also to automatically run this macro so Portfolio P&L can be calculated without any human intervention. (Apple systems might also have something similar to task scheduler that can be utilized)
