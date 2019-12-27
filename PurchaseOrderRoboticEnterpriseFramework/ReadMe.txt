About Purchase Order Bot:

This is an unattended bot which will be used to create Purchase Orders in Apptivo Purchase Order Management system.
The Dispatcher will use the Data\PurchaseOrders.xlsx file to create transactions in UiPath Orchestrator Queue. 
The Transaction will have details like  Supplier,Address,City, State,zip and Item Name. 
Once the Dispatcher run is successful then the user needs to run the Main.xaml (Performer with ReFramework)
The bot will create the Purchase orders in Apptivo ssytem and then update the Purchase Order number in the Data\PurchaseOrders.xlsx file

Pre Requiste:

1. UiPath Studio is installed with Packages :UiPath.Excel.Activities & UiPath.UIAutomation.Activities
2. Create a Uipath Orchestrator account and connect it with the Robot.
3. Create a new Queue item called "PurchaseOrders" in the Orchstrator 
4. Update the Data\Config.xlsx with the Queue name and project name.
5. Update the Data\PurchaseOrders.xlsx with the Transactions details.
6. Get a Apptivo Trial account setup and get access to Purchase Order application
7. Make sure UiPath Chrome Plug in is installed
8. Microsoft Excel application.

Run:
1. Run the PurchaseOrdersDispatcher.xaml from UiPath Studio first to create new Transactions in UiPath Queue.
2. Run the Main.xaml from Uipath studio to create the purchase orders 
3. After the run was successful please check the Data\PurchaseOrders.xlsx file for the Purchase Order numbers.