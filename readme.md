# ParcelDaily API Documentation
Version: v1.0 <br/>
[Technical Documentation](https://parceldaily.docs.apiary.io)
***

## Introduction
Welcome to ParcelDaily API. This API is created for ParcelDaily users to make orders for sending parcels with different choices of courier services provided. It also allows users to track the status of the order or the parcel. The API not only has these functionalities, it as well allows users to perform some other actions mentioned in the following sections. All the JSON files are provided in this repository under `constants` folder.
![ParcelDailyLogo](/images/logo.png "ParcelDaily")

### Outline
- [ParcelDaily API Documentation](#parceldaily-api-documentation)
  - [Introduction](#introduction)
    - [Outline](#outline)
  - [How to Get a ParcelDaily API [Sandbox]](#how-to-get-a-parceldaily-api-sandbox)
  - [How to Get a ParcelDaily API [Production]](#how-to-get-a-parceldaily-api-production)
  - [What Can You Do with the API](#what-can-you-do-with-the-api)
  - [How to Obtain ParcelDaily API Credentials [Production]](#how-to-obtain-parceldaily-api-credentials-production)
  - [How to Top Up Credit](#how-to-top-up-credit)
  - [View My Order](#view-my-order)
  - [Courier-specific Information](#courier-specific-information)
    - [Poslaju](#poslaju)
    - [J&T](#jt)
    - [NinjaVan](#ninjavan)
    - [DHL](#dhl)
    - [CityLink](#citylink)
    - [Pickupp](#pickupp)
    - [Teleport](#teleport)
    - [SF Standard](#sfstandard)
    - [SF Economy](#sfeconomy)
    - [Flash](#flash)
  - [Tracking API](#tracking-api)
  - [Reference](#reference)
   <!-- 3. [`Ninjavan`](###ninjavan)
   4. [`DHL`](###dhl) -->
   <!-- 3. [`CityLink`](###citylink) -->
<!-- 7. [`Reference`](##Reference) -->

## How to Get a ParcelDaily API [Sandbox]
Please contact your account manager to assign a Sandbox **`Token`** and **`Merchant Id`** for your account. If you are here for play around, you can try use this credential for quick test purpose.<br/>
| Merchant Id | Token |
|:------------|:------|
| 8VqGyrqYCQ  | 950af98c-f033-4cdd-ae8a-82db543a3efe |

## How to Get a ParcelDaily API [Production]
Refer and follow the instructions given in the [Technical Documentation](https://parceldaily.docs.apiary.io). It will gives you a clear step-by-step guide.<br/><br/>
![Integration Workflow](/images/integration_workflow.jpg)
## What Can You Do with the API
| Action              | Description                                                                                                 |
|:------------------- |:------------------------------------------------------------------------------------------------------------|
| Rate Checking       | Checks the rate of the delivery fee for different courier services for different region and distance        |
| Make Order          | Make an order with up to 5 choices of courier services to send your parcel to anywhere in the country       |
| Make Bulk Order     | Make an bulk order with up to 5 choices of courier services to send your parcel to anywhere in the country  |
| Checkout order      | Make payment for the order you have made                                                                    |
| Get order status    | Check the order processing status in the courier service                                                    |
| Check parcel status | Check the parcel delivering status                                                                          |
| Tracking            | Track the parcel delivering status from the courier service                                                 |
| Consignment Note    | Download the consignment note through signed URL                                                            |
| PL9 form            | Download the PL9 form when have poslaju parcel pickup through signed URL                                    |

<br/>

<!-- 1. Rate Checking

   >Checks the rate of the delivery fee for different courier services for different region and distance.

2. Make order

   >Make an order with up to 5 choices of courier services to send your parcel to anywhere in the country.

3. Checkout order

   >Make payment for the order you have made.

4. Get order status

   >Check the order processing status in the courier service.

5. Check parcel status

   >Check the parcel delivering status.

6. Tracking
   
   >Track the parcel delivering status from the courier service. -->

## How to Obtain ParcelDaily API Credentials [Production]
After successfully login your account you can get the credential in external api page. To get the token key, you need to click **"Generate Token Key"** button.
You can also enter the URL of your website here if you using **Tracking API**<br/><br/>
![ExternalAPI Page](/images/externalapi.png)

## How to Top Up Credit
1. Register an account at partner.parceldaily.com <br/><br/>
![Register Page](/images/register.gif "Register page")<br/><br/>
2. Login with the account you registered<br/><br/>
![Login Page](/images/login.gif "Login page")<br/><br/>
3. Navigate to the [Top Up](http://partner.parceldaily.com/profile/top-up) page in the side navigation bar **or** 
click on the Top Up button in Dashboard page<br/><br/>
![Navbar TopUp](/images/navbar_topup.jpeg "Top Up page in navigation bar")      ![Dashboard TopUp](/images/dashboard_topup.jpeg "Top Up button in dashboard")<br/><br/>


## View My Order
To view all the order made in ParcelDaily, simply navigate to the [Track Status](http://partner.parceldaily.com/parcel-status) page <br/><br/>
![Track Status Page](/images/trackPage.jpeg "Check all orders")<br/><br/>


## Courier-specific Information
### Poslaju
- Insurance is **NOT** supported
- COD is **NOT** supported
- Drop Off **IS** supported
- The pickup cut-off time is at **12PM**
- No Pick up for now

### J&T
- Insurance **IS** supported
- COD **IS** supported
- Drop Off **IS** supported
- Shipment parcel description is **NOT** supported
<!-- - Minimum for pickup: 5 parcels and above -->

### NinjaVan
- The minimum of character for name are 3 characters
- The maximum of character for name are 30 characters
- Insurance **IS** supported
- COD **IS** supported
- Drop Off **IS** supported
<!-- - Minimum for pickup: 1 parcels and above -->

### DHL
- The minimum of character for name are 3 characters
- The maximum of character for name are 30 characters
- The minimum of character for address lines are 3 characters each 
- The maximum of character for address lines are 50 characters each 
- City are limited to 30 characters
- Parcel detail are limited to 50 characters
- Insurance **IS** supported
- COD **IS** supported
- Drop Off **IS** supported
<!-- - Minimum for pickup: 5 parcels and above -->

### CityLink
- Name are limited to 50 characters
- Address lines are limited to 50 characters each
- City are limited to 20 characters
- Parcel detail are limited to 50 characters
- Insurance is **NOT** supported
- COD is **NOT** supported
- Drop Off is **NOT** supported
<!-- - Minimum for pickup: 1 parcels and above -->

### Pickupp
- **NOT** support parcel weight with more than 10kg
- Insurance is **NOT** supported
- COD is **NOT** supported
- Drop Off is **NOT** supported

### Teleport
- Only for International Country and East Malaysia
- Email is **required** for both sender and receiver
- Insurance is **NOT** supported
- COD is **NOT** supported
- Drop Off is **NOT** supported

### SF Standard
- Only for International Country
- Insurance is **NOT** supported
- COD is **NOT** supported
- Drop Off is **IS** supported
- Commodity Id is **required**

### SF Economy
- Only for International Country
- Insurance is **NOT** supported
- COD is **NOT** supported
- Drop Off is **IS** supported
- Commodity Id is **required**

### Flash
- Insurance is **NOT** supported
- COD is **IS** supported
- Does **NOT** supported COD that have decimal value
- Drop Off is **NOT** supported

##### **ONLY DHL, Ninjavan, J&T and Flash support Cash On Delivery

##### **For international delivery, currently ONLY support Singapore

##### **ALL parcel have auto refund if order fail

## Tracking API
We provide a webhook API only for for **POST** method for tracking of parcels. Once you register a webhook URL with ParcelDaily, we will issue a **HTTP POST** request to the URL
specified every time an event occurs. The request's **POST** parameters will contain JSON data relevant to the event that triggered the request. Below is the sample JSON Output<br/><br/>
![Sample JSON Output](/images/samplejson.png)  
## Reference
Contact <sales@parceldaily.com> for more information and support
