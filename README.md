# Service Oriented Architecture Implementation - WS Discovery + Palindrome Service (JAWX) # 

1. Just import the zip files using Netbeans (File> Import Project> From ZIP).
2. Do it for both ChowdurySevice and ChowdhuryClient and WSDeploy
3. Right click on the ChowdhuryService project and click Deploy to deploy it on the GlassFish server.
4. If you are Windows user you can run the WsDiscovery GUI from command-prompt with the command: 
```javascript
java -jar –Dip=xx wsdiscovery-gui2-1.0-SNAPSHOT-jar-with-dependencies.jar
// Here «xx» is the IP address of the interface, e.g., 10.X.X.X.
```
5. Make sure to insert the scope when you are publishing a new service. Mac users can Publish the Palindrome service using the WsDeploy program attach to this repository. Right click on the project after importing it and click run. When asked for IP address input enter your IP address of the user interface and minimize the program. You can close the WsDeploy program anytime by opening console on IDE and hit return key.
6. Right click on the ChowdhuryClient project and click run. The program will keep searching for the published service in the network using the port type search criteria of "{http://check.palindrome.com/}PalindromeCheck" in every 5 seconds until the published Palindrome service is found. 
7. Insert the string of your choice in the text box to check if the string is a Palindrome. If the service get disconnected from the client you need to rerun the program again.




