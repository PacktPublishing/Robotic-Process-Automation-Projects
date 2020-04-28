About Helpdesk Agent Assisted Bot:

Agent Assistant Robot will trigger the bot with Hotkey keyboard trigger(ALT +S) by the Agent.
The bot will then read the Request.xlsx from the 'Requests' folder,The excel file has the content of the helpdesk ticket.
New workflow called"ReadExcelRequest.XAML" is invoked to read the content of the Excel ticket request file and store those in seperate variables.
The output arguments from this workflow are inputed as the input arguments to the next invoked workflow called "ZohoAutomation.XAML". This workflow will create a helpdesk ticket in Zoho desk application.
Once the ticket is created , the request.xlsx file will be moved to the 'Processed' folder
The Agent can place another 'request.xlsx' file in the Request folder and use 'ALT +S' to create the ticket
The Agent has to use the 'STOP' option in the UiPath Studio to stop the automation.

Pre Requiste:

1. UiPath Studio is installed 
2. Zoho Desk already logged in a Chrome Browser in "Ticket" home page
3. Update the Variable called 'strBrowserTitle' in ZohoAutomation.XAML with the Zoho portal name i.e update the name of your desk inplace of '*HCLTestportal*' (make sure you have the * prefix and suffix)
4. Place a file 'Request.xlsx' file ( you can find a sample input file in the Requests folder)
5. Open the Main.xaml in Studio and Run the automation.
6. Use ALT + S to Trigger the automation and use 'STOP' option in Studio to stop the bot.

Note:
Zoho website will be continously updated if the automation failed then you need to update the selectors used in this project before you try it again. It can be easily performed by just using the "Indicate on Screen" Option"

Depedencies Error and Fix:
If you get a Error when you open the Main.xaml i.e. avtivities are not loaded propoerly. Follow the below steps.
1. Close the main.xaml.
2. Open the ReadExcelRequest.xaml and click fix dependencies issues , you should be able to see the activities in this workflow.
3. Open the ZOHOAutomation.xaml and click fix dependencies issues , you should be able to see the activities in this workflow.
4. Now Open Main.xaml and click fix dependencies issues , you should be able to see the activities in this workflow.
