<h2>Prior to Running the Application</h2>
<details><summary>Click to expand</summary>
<br>
Prior to running the application for any system, one will need to install and set-up an IDE or a code editor that is compatible with TypeScript, JavaScript, HTML and CSS files. Our group predominantly used Visual Studio Code, and further instructions will use that code editor as a reference for installation. However, provided that one's editor or IDE correpsonds with the above requirements and allows for running command terminals within the editor/IDE, the following instructions will be fairly straightforward to follow.<br>
<br>
Prior to opening the application, Node.js and npm command line interface must be installed on your computer.<br>
[This webpage](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm) will provide step-by-step process in order to get both tools on your system.<br>
<br>
Once the requirements above are satisfied, use the IDE/editor to open the g03-code-commander-a/Application/Code-Commander folder.<br>
<br>
You will then need to open a new terminal. Once doing so, you will need to install the following dependencies: <br>
<br>
npm install -g @ionic/cli<br>
ionic start myApp tabs --type react <br>
npm install react <br>
npm install @capacitor/core <br>
npm install @capacitor/cli --save-dev <br>
npx cat init <br>
npm install mapbox <br>
npm install realm-web<br>
npm install axios<br>
npm install --save @mapbox/mapbox-gl-geocoder <br>
npm i react-chartsjs-2 chart.js <br>
npm install @emailjs/browser --save <br>
npm i mapbox-gl-style-switcher --save <br>
npm install jquery <br>
<br>
Gradle will also be needed in order to create mobile builds. You can find instructions on downloading Gradle [here](https://gradle.org/install/).<br>
Once these dependencies are installed, you can move on to the next steps to build and run the program. You will no longer need to install these dependencies after this initial step. <br>
</details>

<h2>Running the Application on Desktop:</h2>
<details><summary>Click to expand</summary><br>
To run and use the application on a web browser on your desktop computer, open the terminal and enter the command 'ionic serve' in the Application/Code-Commander folder. <br>
</details>

<h2>Running the Application on Android/iOS:</h2>
<details><summary>Click to expand</summary> <br>
Prior to running the application on your Android/iOS device, developer options will need to be turned on in order to make a build on your particular mobile device. Use the links below to enable developer options on your chosen device.<br>
<br>
[Turning on developer options for an **Android** device](https://developer.android.com/studio/debug/dev-options)<br>
[Turning on developer options for an **iOS** device](https://docs.testarchitect.com/automation-guide/application-testing/mobile-testing/testing-mobile-applications/ios-automation/setting-up-the-ios-test-environment/setting-up-ios-automation/enabling-development-mode-on-ios-device/)<br>
<br>
Once this has been done, you need to plug in your mobile device onto your desktop computer via USB. Once this is done, open a new terminal and enter the command 'ionic capacitor serve', which will allow you to select the connected mobile device and automatically create a build for the device.<br>
Once a build is completed, the application 'Code-Commander' should be available to run on your device. Simply open it to begin running the application.<br>
</details>
<h2>Creating a Violation</h2>
<details><summary>Click to expand</summary>
To create a new violation, double click on a location on the map and a page will pull up. Select the date that this is occuring on the calender. Select the vioation type(s). Add a picture with the Attach Picture button (currently not functional). Add any notes necessary. Then hit the ADD VIOLATION button. A marker will appear on the map and by tapping the marker, a popup of the information inserted will appear (found in 'Home.js' and 'Violaton-create.tsx'). 
<br><br>
</details>
<h2>Updating a Violation</h2>
<details><summary>Click to expand</summary>
A update a violation, double click on a location that already has a violation entry. A page will pull up. The information of that violation that is editable can be autofilled in the date, violation type, notes section that is similar to the page used to a create violation. The edits can be saved with the SAVE CHANGES button. The violation can be removed by completion with the RESOLVE ALL button. The violation can be deleted with the DELETE ALL button (only use in case of creating a violation that shouldn't be there; 'Home.js' and 'Edit-violation.tsx')
<br><br>
</details>
<h2>Making and Saving a Route</h2>
<details><summary>Click to expand</summary>
To create and save a route that a user takes starts by selecting the tracking location button (under the zoom in and out buttons). Then select the blue play button (blue). Your position will be saved after a certain amount of time is passed or a certain amount of distance is passed (which every comes first). To end the route, hit the stop button (it will be the same location as the initial play button). Your path will be saved and entered into the database (found in 'Home.js')
<br><br>
</details>
<h2>Pulling up a Route</h2>
<details><summary>Click to expand</summary>
To pull up a route, select the red caution sign button (bottom left) and select the car marker icon button (top button). A box will popup that takes an employeeID and a date. Enter the employeeID number and the date the route occurred in the format of YYYY-MM-DD. Then select the SHOW ROUTE button. On the map, the path will appear. The light green marker is the starting point, the dark green marker is the end point, and the red markers are violations the user entered while on their route. The red line is the path on the road the user took (found in 'Home.js').
<br><br>
</details>
<h2>Seeing List of Selected Violations</h2>
<details><summary>Click to expand</summary>
To see a list of Violating address, select the red caution sign button (bottom left) and select the pin marker icon button (second from the top button). Select which violations that you want to look up and scroll down to the bottom. Select the SHOW VIOLATIONS button. All of this occurs on the VioLocation-menu.tsx file). This will take you to a new page that will list out the violation address, number of violations at that address, the values (true/false) of all violation types, the coordinates, and the date that address was added (found in 'showViolations.tsx').
<br><br>
</details>
<h2>Emailing a List of Violations</h2>
<details><summary>Click to expand</summary>
To email a list of the violation, first generate the list using the same method as "Seeing List of Selected Violations" above. On that final page, the top will allow for an email to be entered (which will require an appropriate email format) and send the list using the send email button (found in 'showViolation.tsx').
<br><br>
</details>
<h2>Displaying a Selection of Violations on the Map</h2>
<details><summary>Click to expand</summary>
To display a selection of violations on the map, follow the method as "Seeing List of Selected Violations" above. Then hit the back button. It will return to the map and markers will be placed at every location a violation occurred. By selecting the marker, information popup will appear with the address, number of violations, violation types, picture(s). The markers will display based on the number of violations at that location. If there are multiple violations at that location, the markers will be based on heat. Location with fewer violations will have cooler colors (starting with green at 2) and violations with more violation will have warmer colors (ending at a brown-red at 9). If the location has one violation then it will display the violation symbol with its respective color (a blue house for illegal occupancy use, a yellow hardhat for illegal construction, a pink sign for illegal signage, gray trashcan for sanitation issue, red hammer for maintenance issue, blue eye for visibility issue, flipped red yield sign for right-of-way issue, green paper for permit issue, and purple exclamation point for other; all are found im 'Home.js'). 
</details>
<h2>Making a Graph</h2>
<details><summary>Click to expand</summary>
To make a graph, select the red caution sign button (bottom left) and select the bar graph icon (bottom button). A new page will pull up. Select the graphing button that is desired, select the date range (optional), select the axis option(s), select the viotation types (optional and some axis options will not allow for changes here), and select to show resolved, or only resolved issues (optional). All of these options are in the 'Charts-menu.tsx' file. Once the chart and axis option(s), the GENERATE button will ungray and become enabled. Select the GENERATE button to pull up a new page with the graph (the graphs are one pages called 'barChart.tsx', 'pieChart.tsx', and 'lineChart.tsx').
<br><br>
</details>
<h2>Getting a Navigation Path</h2>
<details><summary>Click to expand</summary>
To get a navigation path (similar to that of navigation apps like Waze, Apple Maps, Google Maps), select the green compass button (bottom left). An A and B box will popup in the top right corner. A is the starting location and B is the destination. A path will appear on the map (found in 'Home.js'). 
<br><br>
</details>
<h2>Location Search</h2>
<details><summary>Click to expand</summary>
At the top is a search bar. Use this search bar to look up an address on the map (found in 'Home.js').
<br><br>
</details>
<h2>Map Editting</h2>
<details><summary>Click to expand</summary>
The top left corner has 5 buttons. From top down, there are the zoom in, zoom out, re-align, tracking, and map change button. The map change button will change the style of the map that is displayed (found in 'Home.js')
<br><br>
</details>
<h2>Changing the Bounds of the Map</h2>
<details><summary>Click to expand</summary>
To change the bounds that the map is constrained by, simply change the 'bounds' const at lines 39-42 of 'Home.js' to your desired coordinates (Southwest and Northeast corners).
</details>
<h2>Realm Functions</h2>
<details><summary>Click to expand</summary>
All the functions and webhooks used can be found in functions.txt and functions.js
<br><br>
</details>

