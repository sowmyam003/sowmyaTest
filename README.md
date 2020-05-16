What the Project :

This a simple automation framework that has been setup to test search for tickets on the trainline website
The Frame has been setup using , Cucumber , TestNg, Selenium/Webdriver , Maven, Selenium Grid

How the user can get started with the Project :

- Check out the Project on your local machine
- Open the Project in Eclipse IDE / intellij
- In the config.properties file update the below properties details related to your selenium grid i.e hub host and port information
hubHost=
hubPort=

Note : To start a selenium grid hub and nodes, follow below steps
- Open cmd
- Goto folder sowmyaTest>> selenium server
- To start selenium hub : Run the command 'java -jar selenium-server-standalone-3.141.59.jar -role hub -port 4445'
- To start selenium node: Run the command 'java -Dwebdriver.chrome.driver="<--Enter path where project is checkedout-->\sowmyaTest\drivers\chromedriver.exe" -Dwebdriver.gecko.driver="<--Enter path where project is checkedout-->\sowmyaTest\drivers\geckodriver.exe" -jar selenium-server-standalone-3.141.59.jar -role node -port 5556 -hub "http://localhost:4445/grid/register/"'




For running a scenario ,you can use below ways:
- Please go to the SearchTrainTickets.feature and run scenario as cucumber test
or
- Run TestRunner.java as a TestNG test
or 
- Run pom.xml file as a maven test 

Test Results Report: 

once the test runs the Result Report will be generated in the target/cucumber
