# ModusBox Mojaloop Lab
## Getting started with the Lab


## 1.0 Obtaining an Access Token

- 1.1 Go to the public gateway (the link has been removed as this environment is not public).

![lab_onboarding_01](./images/lab_onboarding_01.png)


- 1.2 Click “Sign Up”, and go through the steps to create a new account

![lab_onboarding_02](./images/lab_onboarding_02.png)


- 1.3 Click “Sign Up” > follow the dialog box to the sign in page > Enter your details and “Sign In”

![lab_onboarding_04](./images/lab_onboarding_04.png)
![lab_onboarding_05](./images/lab_onboarding_05.png)


- 1.4 In the top left, select “Applications”

![lab_onboarding_06](./images/lab_onboarding_06.png)


- 1.5 Select “Default Application” from the list

![lab_onboarding_07](./images/lab_onboarding_07.png)

- 1.6 Navigate to “Production Keys” > set the validity of the key to “-1” > “Generate Keys”

![lab_onboarding_08](./images/lab_onboarding_08.png)
![lab_onboarding_09](./images/lab_onboarding_09.png)

- 1.7 Your access key along with a token will be created. Click “Show keys”

![lab_onboarding_10](./images/lab_onboarding_10.png)

- 1.8 Observe that your access token has been created. You can copy this for later reference

![lab_onboarding_11](./images/lab_onboarding_11.png)

- 1.9 Navigate to APIs in the top left menu

![lab_onboarding_12](./images/lab_onboarding_12.png)

- 1.10 From the list of APIs, select “CentralLedgerApi…”

![lab_onboarding_13](./images/lab_onboarding_13.png)


- 1.11 You now need to subscribe the DefaultApplication to this api. You can do this in the top right > “Subscribe”

![lab_onboarding_14](./images/lab_onboarding_14.png)
![lab_onboarding_15](./images/lab_onboarding_15.png)


- 1.12 Navigate to “Api Console”. Your access token should already be pre-filled for you.

![lab_onboarding_16](./images/lab_onboarding_16.png)

- 1.13 Now we can test out the `/health` endpoint of the central-ledger service. Browse down the list of endpoints > “Try it out” > “Execute”

![lab_onboarding_17](./images/lab_onboarding_17.png)
![lab_onboarding_18](./images/lab_onboarding_18.png)
![lab_onboarding_19](./images/lab_onboarding_19.png)



1.14 You should see a response similar to the following:


```json
{
  "status": "OK",
  "uptime": 535767.333,
  "startTime": "2019-09-17T15:11:37.794Z",
  "versionNumber": "7.3.1",
  "services": [
    {
      "name": "datastore",
      "status": "OK"
    },
    {
      "name": "broker",
      "status": "OK"
    }
  ]
}
```