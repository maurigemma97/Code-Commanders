<h1>Synopsis</h1>
<details>
This Application called Code Commander is an app that would be used on tablets (both iOS and Android) for Bowling Green Code Enforcement Officers, primarily, and other Bowling Green City Officials, secondarily. Bowling Green Code Enforcement Officers can use this app while they are driving through the city to take down the details at that location and have it enter the database immediately and can have the locations updated and removed from the database as seen necessary (if location has/have fixed the violation(s)). Bowling Green Code Enforcement Officers or other Bowling Green City Officals can review the violations that are occurring in the city to see if there are trends in the city based on time and/or location. The app can also be used to save the work of Code Enforcement Officers to save their work efficiency. 
</details>

<h1>Motivation</h1>
<details>
Currently Bowling Green Code Enforcement Officers use pen and paper to take down the details of locations with code violations and when they return to their office, they have the violations entered into their system. This system works, but is inefficient and susceptible to potential errors. Papers are easy to lose in transit and this process takes a long time. This application is meant to help make Code Enforcement Officers's jobs easier and faster. Instead of pen and paper and entering in the system at the office, Code Enforcement Officers use the app to enter the location into the database while they are at the location. Nothing can be lost in transit and this process is much faster. This also acts as an app the city can review for trends in their violations and for Code Enforcement Officers Supervisors to review work performance. 
</details>

<h1>Installation and Testing</h1>
<details>
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
</details>

<h1>API Reference</h1>
<details>
Database:
Atlas: https://www.mongodb.com/atlas/database <br/>
Serverless Backend:
Realm: https://www.mongodb.com/realm 
</details>

<h1>Authors</h1>
<details>
Nicholas Acuncius - nacunci@bgsu.edu <br/>
Matthew Aurigemma - aurigem@bgsu.edu <br/>
Evan Buchanan - erbucha@bgsu.edu <br/>
Jackson Conrad - jwconra@bgsu.edu <br/>
Caleb Courtney - clcourt@bgsu.edu <br/>
Jaxsin Power - jxpower@bgsu.edu
</details>

<h1>Acknowledgments</h1>
<details>
This application was created as a Capstone Project with Bowling Green State University. <br>
  Thanks to Dr. Jerry Wicks for sponsoring the creation of this application and acting as the client of the application. <br>
  Thanks to Dr. Tianyi Song and Dr. Joseph Chao for being the Project Managers. <br>
  Thanks to Bowling Green State University for the opportunity towards creating this application. <br>
</details>
