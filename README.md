I have added project into the GitHub.Steps to download:
1. Copy the Github project URL.
2.Clone it your local.

I have automated the given scenario using ROBOT FRAMEWORK.

Project overview:
 1. Created a project "JustEat" in Pycharm 

 2. Project has three Directories - Resources , Tests and Results

 3. Resources has one Directory - PageObjects ,DataFile and one Keyword Files

 4. Resources/PageObjects Directory has two Page Object files.
    1. LandingPage.robot 
    2. SearchResultPage.robot 

 5.One Keyword files under Resources directory are:
     1. CommonKeywords.robot : It has keywords for Test Setup and Test Teardown.

 6. Tests Directory has one file JustEat.robot . The test script is written in this file.Test case consist of three keywords:
    1. The application Loads Correctly - Here I am waiting till the Just Eat Logo and Search window is displayed.
    2. User searches for Restaurants by Postal code 
    3. User should see some Restaurants in Search Results - 
	Here I am checking page is loaded, if the number of open restaurants is more than 10 , list of restaurants is displayed and restaurants rating icon  is present for open restaurants.

 7. I am using Results Directory for reports.

 8. PostalCode is driven using Excel File(Testdata.xlsx).TestDataExcel.robot file in Resources directory will read the data from excel sheet.

To Run test script :
1.Go to cmd
2. Navigate to the project folder by using 'cd' command and type robot -d Results tests/justEat.robot

To check Reports:
- Open Pycharm and go to Results Directory
- Under Results Directory , right click on report.html file
- Select option "Open in Browser" and select Browser


