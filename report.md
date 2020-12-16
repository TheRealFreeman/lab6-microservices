## Activities:

* **The two microservices accounts (2222) and web are running and registered (two terminals, logs screenshots):**

Accounts service running on port 2222:
![accountLogs](screenshots/accountLogs.png)
      
Web service running on port 3333:
![webLogs](screenshots/webLogs.png)


* **The service registration service has the two microservices registered (a third terminal, dashboard screenshots):**

Registration server running on port 1111:
![registrationLogs](screenshots/registrationLogs.png)

Registration dashboard:

![registrationDashboard](screenshots/initialDashboard.png)

* **A second account microservice is running in the port 4444 and it is registered 
(a fourth terminal, log screenshots).**

Second account service running on port 4444:
![secondAccountService](screenshots/secondAccountsService.png)

Dashboard showing the second account service is running and registered:

![twoAccountsDashboard](screenshots/2accountsDashboard.png)


* **What happens when the microservice running on port 2222 is killed? Can the web service provide information
about the accounts and why?**

Dashboard after service is killed:

![finalDashboard](screenshots/finalDashboard.png)

After killing the microservice, it is removed from the registered applications list of the dashboard, nevertheless,
since there is another instance of the accounts service running (the one on port 4444) the web service can still 
provide information about the accounts using that second microservice instance. 
