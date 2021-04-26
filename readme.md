# ParcelDaily API Documentation
Version: v0.1
[Technical Documentation](https://parceldaily.docs.apiary.io)
***

## Introduction
Welcome to ParcelDaily API. This API is created for ParcelDaily users to make orders for sending parcels with different choices of courier services provided. It also allows users to track the status of the order or the parcel. The API not only has these functionalities, it as well allows users to perform some other actions mentioned below. 
![ParcelDailyLogo](/images/logo.png "ParcelDaily")

### Outline
1. [`How to Get a ParcelDaily API`](##How-to-Get-a-ParcelDaily-API)
2. [`What Can You Do with the API`](##What-can-you-do-with-the-api)
3. [`How to Top Up Credit`](##How-to-Top-Up-Credit)
4. [`View My Order`](##View-My-Order)
5. [`Integration workflow`](##Integration-workflow)
6. [`Courier-specific information`](##Courier-specific-information)
   1. [`Poslaju`](###poslaju)
   2. [`J&T`](###j&t)
   3. [`Ninjavan`](###ninjavan)
   4. [`DHL`](###dhl)
   5. [`CityLink`](###citylink)
7. [`Reference`](##Reference)

## How to Get a ParcelDaily API
Refer and follow the instructions given in the [Technical Documentation](https://parceldaily.docs.apiary.io). It will gives you a clear step-by-step guide.

## What Can You Do with the API
| Action              | Description                                                                                           |
|:------------------- |:----------------------------------------------------------------------------------------------------- |
| Rate Checking       | Checks the rate of the delivery fee for different courier services for different region and distance  |
| Make Order          | Make an order with up to 5 choices of courier services to send your parcel to anywhere in the country |
| Checkout order      | Make payment for the order you have made                                                              |
| Get order status    | Check the order processing status in the courier service                                              |
| Check parcel status | Check the parcel delivering status                                                                    |
| Tracking            | Track the parcel delivering status from the courier service                                           |

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

## How to Top Up Credit
1. Register an account at partner.parceldaily.com <br/><br/>
![Register Page](/images/register.gif "Register page")<br/><br/>
2. Login with the account you registered<br/><br/>
![Login Page](/images/login.gif "Login page")<br/><br/>
3. Navigate to the [Top Up](http://partner.parceldaily.com/profile/top-up) page in the side navigation bar **or** 
click on the Top Up button in Dashboard page<br/><br/>
![Navbar TopUp](/images/navbar_topup.jpeg "Top Up page in navigation bar")   ![Dashboard TopUp](/images/dashboard_topup.jpeg "Top Up button in dashboard")<br/><br/>


## View My Order
To view all the order made in ParcelDaily, simply navigate to the [Track Status](http://partner.parceldaily.com/parcel-status) page <br/><br/>
![Track Status Page](/images/trackPage.jpeg "Check all orders")<br/><br/>


## Courier-specific Information
### Poslaju
- The pickup cut-off time is at **12PM**

### J&T
- The order response takes comparatively longer time than other courier services
- City name Padang Besar Utara need to change into Padang Besar
- All postcode in Ipoh area are 31650 (e.g: 31500 -> 31650)
- Shipment parcel description is **NOT** supported

<!-- ### NinjaVan
- Generation of API token is limited to **10 times** per minute, else one will be blocked for 1 hour
- Token validation period is dynamic ranges between 1 hour and 30 days
- A new OAuth access token will be generated automatically 5 minutes before the token expires -->

<!-- ### DHL
-  -->

### CityLink
<!-- - The token renew every 7 days -->
- Address lines are limited to 50 characters each
<!-- - **DOES NOT** return error state, errors are reflected in the return code and return message in success state
- Connote is given in base64 binary form therefore conversion is required to get the pdf version -->

## Reference
Contact <sales@parceldaily.com> for more information and support