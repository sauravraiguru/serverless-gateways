# Serverless and API Gateways - Lab

###  Welcome to this serverless and Cloud API Gateways Lab, where we will be trying out `actions` , `triggers` and exposing & securing actions using `API gateways`


## 1. Creating API Gateways service.

Go to API Gateways service page on IBM Cloud and `Create` a service.

https://cloud.ibm.com/catalog/services/api-gateway

Note: This service is available in Lite plan only.


## 2. Let us create our first function on a NodeJS runtime.

A. Go to -> https://cloud.ibm.com/functions/ and Click on `actions`

![Actions](images/actions.png)

B. lets create our first action as below and click on `Create`

![Create Action](images/create-action.png)

C. Lets try out if the action is working now,
-> Go to `Endpoints` on the left bar and copy the CURL command at bottom


![Endpoints](images/endpoints.png)


and paste in the terminal or prompt.
Alternatively you can also try web-action to check it. You will see `hello world` message in the JSON response.

![curlcommand](images/curl.png)


## 3 Enabling actions as a `trigger` [Optional]
Click on `connected triggers` on the left bar and select `Add Trigger` to quickly create an event based trigger.

![Trigger](images/triggers.png)

There are many ways to trigger based on an event type, but we will choose a time-based `periodic` trigger

![Periodic trigger](images/periodic.png)
a. Provide a `trigger name` say `sample` a cron for every minute and click on `Create & Connect`

![Trigger Config](images/create-trigger.png)

Once create this trigger will be invoked every minute (as per the rule) and we can see the same in Function Dashboard
[Functions Dashboard](https://cloud.ibm.com/functions/dashboard)


## 4. Exposing this function as a secure API & manage it using API Gateways
We need to now expose our actions as API and also secure them
-> lets go to API gateways service which we have created already earlier.
[API Management Service](https://cloud.ibm.com/functions/apimanagement)

Click on

![Trigger Config](images/apimanagement.png)






## 5. [Practice] with variables / parameters





## 6. Additional lab

[create & manage APIs using API Connect](https://developer.ibm.com/tutorials/create-and-manage-apis-using-api-connect/)
