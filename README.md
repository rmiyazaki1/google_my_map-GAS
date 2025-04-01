# google_my_map-GAS
Link Google Spreadsheets and Google My Maps via GAS and KML
#English
1. Prepare your spreadsheet
Open Google Spreadsheet and set up the following columns:
Column A: Point name
Column B: Address
Column C: Latitude
Column D: Longitude
Column E: Point color (red, blue, green, yellow, purple, orange)
Enter the header in the first row (e.g. "Point name", "Address", "Latitude", "Longitude", "Color")
Enter the actual data from the second row onwards

2. Prepare My Maps
Access Google My Maps
Create a new map or select an existing map
Copy the part after "mid=" from the map URL (this is the map ID)

3. Set up Google Apps Script
In the spreadsheet, click "Extensions" → "Apps Script"
In the newly opened script editor, delete all existing code
Paste the script code provided
Change the MY_MAP_ID variable in the script to the map ID you copied earlier
Click the "Save" button (enter any name when asked for a name)

4. Script execution and menu display
In the script editor, select onOpen from the function dropdown
Click the "Execute" button (permissions must be approved the first time)
Return to the spreadsheet and refresh the page (F5 key)
A menu called "Google Maps" will appear at the top of the screen
If the menu does not appear:
In the script editor, add onOpen(); to the last line, save it, and run it again
Or run the updateMyMap function directly in the script editor

5. Creating and importing a KML file
Click "Create KML file" from the "Google Maps" menu in the spreadsheet
If the menu does not appear, run the updateMyMap function directly in the script editor
The script will run and a pop-up will appear with a link to the KML file and instructions
Click the My Maps URL displayed in the pop-up
Click the "+" button for layers on the My Maps screen
Select "Import" and select the generated KML file from Google Drive
The KML file can be accessed from the link displayed in the pop-up
Once the import is complete, the points entered in the spreadsheet will appear on the map

6. Procedures for updating data
Update and add data in the spreadsheet
Click "Google Maps" menu → "Create KML file" again
Import the newly generated KML file to My Maps using the same procedure
Notes
Be sure to enter the point name in the spreadsheet (blank rows will be skipped)
Enter latitude and longitude as numbers
Enter the color as red, blue, green, yellow, purple, or orange (case is not important)
The KML file is saved in Google Drive, so you can also check the history of past updates
This method makes it easy to update data from a spreadsheet to My Maps.
