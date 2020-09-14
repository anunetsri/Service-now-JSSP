# JSSP-ServiceNow
 
 ## JSSP Broker for ServiceNow API
 Sample K2 JSSP Broker connecting K2 to ServiceNow based on [ServiceNow API](https://developer.servicenow.com)
 

This is only a sample broker and is not supported by the product team.
 
 ***Use this code at your own risk, Happy Coding.***
  
 ## Features
 This broker currently supports the followings:
 
 ### ServiceNow [Incidents Entity](/api/now/v1/table/incident)
 - ListIncidents: List all incidents
 - GetIncident: Get details of an incident based on incident ID
 - CreateIncident: Create a new incident
 - UpdateIncident: Update an existing incident
 
Additional Information:  [API Reference](https://developer.servicenow.com/dev.do#!/reference/api/orlando/rest/c_TableAPI)

## What is required to create a K2 Service Instance:
- ServiceNow instance hostname
- Use Static Authentication type and enter username and password for the service instance.

If you don't have an instance of ServiceNow to connect to, you'll need to create a developer account on [ServiceNow Developer Portal](https://developer.servicenow.com)


## To deploy the broker to a K2 Nexus platform
To deploy this broker you can use the bundled JS file under dist folder. Follow the [product documentation here](https://help.k2.com/onlinehelp/platform/userguide/current/default.htm#../Subsystems/Default/Content/Extend/JS-Broker/JSSPRegister.htm%3FTocPath%3DDevelop%7CExtending%2520the%2520K2%2520Nexus%2520Platform%7CCustom%2520Service%2520Types%2520with%2520the%2520JavaScript%2520Service%2520Provider%2520(JSSP)%7C_____8) to deploy the bundled js file to your K2 Nexus instance

## To modify this broker for your use cases:
1. Download this repository
2. Run "npm install"
3. Modify the code in index.ts under the src folder
4. Then run "npm run build" to generate a new bundled JS file for deployment.
