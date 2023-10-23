# Project for opening mass tickets within KIRK.

Before starting to talk about the code, it was developed in JS so that it only works within Google Sheets AppScript.

The Main.JS file, when placed within AppScript, must be named Codigo.gs.

## How it works?

The program aims to open several mass payment calls, aiming to gain performance.

- He receives a connection with Kirk's system where he brings all the necessary fields to open a ticket.
- Then fill in the necessary fields to open tickets as necessary for that type of document.
- The system has a part where you can get several links to the invoices according to the document number entered in field J, where it checks the folder that was entered with its key in the search field and searches for the title of the document within the folder.
- The NF Link field is mandatory, otherwise it will give an error.
- After filling in all the necessary fields, you will need to instantiate the process to go up to Kirk and open the tickets.
- After the ticket is opened, the system will take the link provided in the spreadsheet and make a copy in a shared driver within Google Drive renamed with the IDK generated in the ticket plus the document number, informed in column J.
- If everything goes well, the IDK number will appear in the 'SUCCESS' tab in green, if there is an error, the error message will appear in the column informed.
