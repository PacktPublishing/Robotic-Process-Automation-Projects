About CRMAutomation Bot:

The Bot needs to be run from the UiPath Studio and we will use Google Chrome Borswer for this automation.
The user needs to request trail access to Apptivo CRM from https://www.apptivo.com/ and https://www.crunchbase.com/ - which provides company details.
The User must login to both these sites as the login part of scoped out this project. In addition to his user needs to create 3 Customers in Apptivo CRM.
The Bot will open the existing Apptivo CRM application and read the Customers list and then it opens the Crunchbase site to extract the website, Facebook, LinkedIn and Twitter details.
Once the details are gathered , the bot will automatically update the same details in the Apptivo CRM. 

Pre Requiste:

1. UiPath Studio is installed 
2. User has trail access to both Apptivo CRM and Crucnbase site
3. Apptivo CRM already logged in a Chrome Browser. 
4. Crunchbase.com site page is closed in Browser.
5. Only the Customer names are filled in the Apptivo CRM.

Depedencies Error and Fix:
If you get a Error when you open the Main.xaml i.e. avtivities are not loaded properly. Follow the below steps.
1. Close the main.xaml.
2. Open the RequestCustomerDetails.xaml and click fix dependencies issues , you should be able to see the activities in this workflow.
3. Now Open Main.xaml and click fix dependencies issues , you should be able to see the activities in this workflow.