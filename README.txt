Instructions to run the automation:

1) Install Java
	java -version
	java version "1.8.0_281"
	Java(TM) SE Runtime Environment (build 1.8.0_281-b09)
	Java HotSpot(TM) 64-Bit Server VM (build 25.281-b09, mixed mode)
2) Install node
	node --version
	v14.16.1
3) Traverse inside the folder Gelato
4) Install the dependencies by following command:
	npm install
5) Once the dependencies are installed, run the tests using below command:
	npm run test
6) From root folder location, run below command to generate report:
	node cypress/cucumber-html-report.js 
7) Results can be checked at report location
	.\cypress\report\index.html
========================================================================

The automation uses cypress tool. Test cases are written in JavaScript with Mocha framework and Chai assertions
Follow the instructions above to run the automation.
Test cases are specified in cypress\integration folder.
Tool uses mochawesome-report tool for generating report.
Since the application under test is a simple application with a single page and not many complicated workflows, I have chosen the mocha framework. It is easier to write shorter test cases with assertions in mocha.
The automation tries to cover different positive and negative test cases. Please refer TestCases.txt for the same. 
The html report generated gives an idea of the test cases that ran along with success and failures.
Also there is one negative test case(Test case no.14)that fails. This is because we have a bug in the application.