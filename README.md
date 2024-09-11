
Youtube video on how to download the tdl and work

[https://www.youtube.com/watch?v=_6P8CVysKsk] (https://www.youtube.com/watch?v=_6P8CVysKsk)



# TallyConnector-V3.0


The TDL Helps to Get Around 75 % of the Data in Tally to Excel in quick seconds in 3 Tables


***Click to download the Connector from Here***

[https://techca.app/viewtopic.php?t=29](https://techca.app/viewtopic.php?t=34)



# Tally-Excel- PowerBI- Power Query ODBC Connector

This Tool will help to import Tally Data (Master Data and Transactional Data) to excel /Power BI/ Power Query.

# Steps in Connecting the TDL In Tally and Import in Excel
**Step 1**
Download the File Named Connection.tcp and paste in any folder in your PC

**Step 2** **Connecting TDL**
Copy the Folder path and Load Any company in Tally and Navigate to F1 Help >> TDL's & Addons
or Press Ctl + Alt + T in Gateway of Tally Menu

![image](https://github.com/ramajayam-CA/Tally-Connector/assets/12751693/6ccaaf4b-13a6-4dad-9924-75402d64976e)

Then Press F4 and Paste the path and select the Connection.tcp File

![image](https://github.com/user-attachments/assets/da0a9949-3475-4af2-bd8c-439e541bb93d)


**Step 3** **Enabling ODBC in Tally**

Navigate to F1 Help >> Settings >> Connectivity and Press Enter

![image](https://github.com/ramajayam-CA/Tally-Connector/assets/12751693/3002cd7d-c011-416a-96de-0141e26ccb0d)


Then Set the Following Options

Tally prime act as : **Both**

Enable ODBC  : **Yes**

Port : 9000 or any other port of your choice

![image](https://github.com/ramajayam-CA/Tally-Connector/assets/12751693/512921e5-1acd-467b-867f-7e1818cf2dfe)


# How to Connect to  Excel through Microsoft Query


**Step 4** 
  **Running Tally in Administrator Mode**

  - After connecting the TDL file, Make sure You have Completed Step 1 to 3 as above  Enabling ODBC **RUN TALLY IN ADMINISTRATOR MODE IN WINDOWS**
  - Then Open Excel and Navigate to Data >> Get Data >> Other Sources >> Microsoft Query >> Then Click on **TALLYODBC_9000** press **OK** in the Choose Data Source
    If you have any error in this step then please go through Steps 1 to 3 properly

![image](https://github.com/ramajayam-CA/Tally-Connector/assets/12751693/c44ffadb-1380-4ab1-af32-041671d0fb75)


![image](https://github.com/ramajayam-CA/Tally-Connector/assets/12751693/1a3de0f6-4156-4cc1-8722-ec969b1807b1)


Refer to the Following link if Microsoft query is not appearing

https://answers.microsoft.com/en-us/msoffice/forum/all/microsoft-query-missing-in-excel-365-how-to-solve/17ce69ec-e8e4-4921-905c-e9c0a6f4b0f2


**Step 5** 

**Selecting the Table in the tally database**

**The following tables** one by one 

**1. A_Sirc_Leder_Detailed_7_1 - Master Data**
**2. A_Sirc_Vourcher7_1        - Transaction Data**

After Selecting press the > button to load all the fields or the selected field 
Then Click **Next** 3 times And finally Click Finish so that the data loaded in Excel 

![image](https://github.com/user-attachments/assets/43a4762f-7428-468b-95a1-78ad94db3f9f)


![image](https://github.com/ramajayam-CA/Tally-Connector/assets/12751693/6756dfcb-e186-41dc-a17c-8f06327a16af)



**For Doubts in connecting to excel refer to the tally documentation**


https://help.tallysolutions.com/tally-prime/data-exchange-tally-prime/extracting-master-data-to-microsoft-excel-using-odbc-tally/


# Tdl Documentation - Community Version 7.1 (For ICAI Members)


Tally Definition Language (TDL) is the development language of Tally Products. TDL is developed to provide the user with the flexibility and power to extend the default capabilities of Tally, and integrate them with the external applications. TDL provides a development platform for the user. The entire user interface of Tally.ERP 9 is built using TDL. TDL as a language, provides capabilities for Rapid Development, Rendering, Data Management, and Integration.

**TDL Can Help Chartered Accountants in the following Ways**

1. Ability to generate Custom reports from Tally 

2. Real-Time integration with Excel / PowerBi / Tableau with the ODBC Access

3. Reduce the time to prepare Fianancial Statements from Tally.

4. Identify 269SS and 269T Transaction in Tally

5. Complete GST Audit in less than 30 Minutes from Tally.

6. Ledger Scrutiny With Advanced filters in Tally

7. Do ageing analysis from a partly Bill reference enabled enviornment.

8. Get All Transaction and Ledger Data in Excel (Even a Very Large Data) in few clicks

9. Get Critical Data Analysis for Tax audit Report

10. Analyse the Utilusation of Funds in a business enviornment.

11. There are many further Benifits being explored by the Author


# Fields Present in the Ledger Table 

![image](https://github.com/user-attachments/assets/cb7e33b8-0975-48f3-9d60-4b1f179ecf4c)



# Fields Present in the Transaction Table. - Daybook

![image](https://github.com/user-attachments/assets/64f3a1bb-e1a6-405b-b822-d939969d2e4e)




# How to Connect to PowerBI


![image](https://github.com/ramajayam-CA/Tally-Connector/assets/12751693/a919eddb-8cc4-4fd7-9811-579bfc8ffa00)

For Doubts in connecting to excel refer to the tally documentation


https://help.tallysolutions.com/tally-prime/data-exchange-tally-prime/extracting-master-data-to-microsoft-excel-using-odbc-tally/


# Important Queries from the above data source - Transactions


SELECT $Key, $MasterId, $AlterID, $VoucherNumber, $Date, $VoucherTypeName, $Led_Lineno, $Type, $LedgerName, $Amount, $Led_Parent, $Led_Group, $Party_LedName, $Vch_GSTIN, $Led_GSTIN, $Party_GST_Type, $GST_Classification, $Narration, $EnteredBy, $LastEventinVoucher, $UpdatedDate, $UpdatedTime, $Nature_Led, $Led_MID, $CompanyName, $Year_from, $Year_to, $Company_number, $Path
FROM A__DayBook


# Important Queries from the above data source - Master data - Ledger


SELECT $Name, $_PrimaryGroup, $Parent, $OpeningBalance, $ClosingBalance, $_PrevYearBalance, $IsRevenue, $PartyGSTIN, $MasterId, $AlterID, $Nature_Led, $UpdatedDate, $UpdatedTime, $CreatedBy, $CreatedDate, $AlteredDate, $AlteredBy, $LastVoucherDate, $CompanyName, $Year_from, $Year_to, $Company_number, $Path
FROM A__M_Ledger


# Get the List of ledgers with forensics data

Select $Name, $Createdby, $CreatedDate, $Masterid, $Alterid, $Alteredon, $Alteredby, $Updateddatetime, $LastVoucherDate, $Parent, $_PrimaryGroup, $$AscrAmt:$openingBalance, $$AscrAmt:$_ClosingBalance from ledger order by $Alterid desc




# TallyNaturalLanguage


This concept was built using [Natural Language in Tally ](https://help.tallysolutions.com/article/te9rel55/SMS/Natural_Language.htm?)

Suggest us for more such prompts [Here](https://docs.google.com/forms/d/e/1FAIpQLScPuohVo0f1tTIkEXSyr5pmgzD4OwbzTay8ONlSE_DRDGbt2Q/viewform)

## The following Prompts will work in the demo


### 1. Ledger Creation 

**```Without mentioning Group Name```**

 - Create Ledger Kavilan
 - Create Ledger ICAI


**```With Group Name```**

Create Ledger Kavilan SundryDebtors

***```With Opening Balance```**

Create Ledger server02 fixedassets -15000
Create Ledger icai sundrycreditors 15000


### Transaction creation

Make Payment 3000 to ICAI

### Stock Creation

Create Item DustCovers FinishedGoods Nos 10 550

### Sales Order

Create SO <PartyName> <Order Reference No> <ItemName 1> <Qty 1> <Amount 1> <ItemName 2> <Qty 2> <Amt 2> ...... <ItemName n> <Qty n> <Amt n>

Create SO Kavilan PO1101 MotherBoard 15nos 10000

Create SO Kavilan PO1102 AssembledPIV 10 25000 MotherBoard 15nos 10000 DustCovers 8 500

