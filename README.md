The Test data can be kept in the fixtures folder under the testData.json file. Data like username, password can be stored here.
The Regression test file under the Integration folder is were tests are written.
The Page Objects houses all the objects in a Page, it is best to havve multiple pages under this folder.Objects like textboxes, buttons etc can be stored here.
The commands.js files have the functions to be used in test which is under the Support folder. Actions like clicks, input etc can be stored here.
The index.js under the support folder is were the command.js commands are imported.
The cypress.json file has the environmen variables(url reporter and test data) with the project settings including timeouts. Also the project id can be found here for ci/cd reports.
Under package.json, the scripts have the config of how tests can be run. The script for dashboard reporting is were integration is done for runs to be published in the dashboard.
Using npm test recordDashboardTest, test is run and pushed to your dashboard, note before you can have visibility to your dashboard, sign into github from cypress test run to fetch project id and dashboard run key.
Mochasome reports for reporting, can be installed using npm install --save-dev mochawesome and npm install --save-dev mocha