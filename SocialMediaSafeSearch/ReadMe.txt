About Social Media SafeSearch Bot:

This is an unattended bot which will search the Input folder for images of JPG or PNG format , and create the list of file paths in the output excel file.
The bot then utilizes the Google vision API activities to use the safe search feature to get the likelihood of Adult, Violent, Racy or Medical Content and then updates the results in the output excel file. 
Then the Administrator can then use the output file to moderate the Images.

Pre Requiste:

1. UiPath Studio is installed with Packages :Uipath.Credentails.Activities , UiPath.GoogleVision.Activities & UiPath.Excel.Activities
2. Input Folder with few images of JPG or PNG format.
3. Output Folder with a Excel file called "ImageDetails.xlsx" (with these columns : ImagePath |	Adult |	Violence |Racy |Medical )
4. Enable Google Vision API in Google developers cloud portal 
5. Google Vision API authetication Google Client ID and Google Secret Key
6. Microsoft Excel application.

Depedencies Error and Fix:
If you get a Error when you open the Main.xaml i.e. activities are not loaded propoerly. Follow the below steps.
1. Close the main.xaml.
2. Open the BuildExcelList.xaml and click fix dependencies issues , you should be able to see the activities in this workflow.
3. Open the GetAppCredentials.xaml and click fix dependencies issues , you should be able to see the activities in this workflow.
4. Open the ReadConfig.xaml and click fix dependencies issues , you should be able to see the activities in this workflow.
5. Open the SafeSearch.xaml and click fix dependencies issues , you should be able to see the activities in this workflow.
6. Now Open Main.xaml and click fix dependencies issues , you should be able to see the activities in this workflow.