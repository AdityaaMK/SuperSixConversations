## SuperSixConversations

- Conversation automation script for Super Six RA staff, only works for Super Six staff.
- Reads a qualtrics form and fills out conversation data with residents.

# Setup and Usage

**How to download**  
On this page, find the code button and then either download the zip file or use git clone in your terminal to place the repository where you please.

**Modules needed to be installed**  
You need to install all these libraries using pip/pip3 or you can set up a virtual environment with these libraries.

- selenium
- xlrd2
- datetime
- chromedriver-binary-auto

**Declaring the spreadsheet with the information**  
Below is the template for how to fill out the data for the script. Please follow it exactly and make sure that the data is in the correct format (date column is formatted to date, etc.). After, you fill it out, download the file and make sure it is named conversations.xlsx and placed in the same directory/folder as the code (you can change the directory to the file in excel_reader.py)

https://docs.google.com/spreadsheets/d/16Dz5gRLQUqZ6qLrWjEvd_B2steo0TlQLvCoelLU0BR8/edit?usp=sharing

# Modifications

The only two files that you would need to modify is the convo_script.py or
the excel_reader.py and the locations are all marked with the comment of "#TODO"

**In convoscript.py**

- want_email in the convo_script.py is personal preference. Set this value to true if you would like to recieve a confirmation email and make sure to input your email in the spreadsheet. If you do not, the script will throw an error at runtime.

**In excel_reader.py**

- loc in excel_reader will change where the directory is for the excel file containing the list of residents and information
