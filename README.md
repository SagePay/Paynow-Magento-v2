Netcash Pay Now Credit Card Payment Module for Magento v2+
=======================================================

Revision 1.0.0

Introduction
------------
A credit card module to take credit card transaction for Magento using Netcash South Africa's Pay Now gateway.

Installation Instructions
-------------------------
Download the files from GitHub:

> https://github.com/Netcash-ZA/Paynow-Magento-v2/archive/master.zip

1. Setup **ZAR** on your Magento site. In the admin panel navigate to 'Stores', and add ZAR under currency Symbols and Rates.
2. Copy the Paynow app folder to your root Magento folder.
    This will not override any files on your system.
3. You will now need to run the following commands in the given order:
    - php ./bin/magento module:enable Paynow_Paynow
    - php ./bin/magento setup:di:compile
    - php ./bin/magento setup:static-content:deploy
    - php ./bin/magento cache:clean
4. Log into the admin panel and navigate to Stores > Configuration > Sales > Payment Method and click on Paynow
5. Enable the module, as well as debugging.
6. Add your Pay Now Service Key
7. Click 'Save Config'

Configuration
-------------

Prerequisites:

You will need:
* Netcash account
* Pay Now service activated
* Netcash account login credentials (with the appropriate permissions setup)
* Netcash - Pay Now Service key
* Cart admin login credentials

A. Netcash Account Configuration Steps:
1. Log into your Netcash account:
	https://merchant.netcash.co.za/SiteLogin.aspx
2. Type in your Username, Password, and PIN
2. Click on ACCOUNT PROFILE on the top menu
3. Select NETCONNECTOR from tghe left side menu
4. Click on PAY NOW from the subsection
5. ACTIVATE the Pay Now service
6. Type in your EMAIL address
7. It is highly advisable to activate test mode & ignore errors while testing
8. Select the PAYMENT OPTIONS required (only the options selected will be displayed to the end user)
9. Remember to remove the "Make Test Mode Active" indicator to accept live payments

* For immediate assistance contact Netcash on 0861 338 338

10. Click SAVE and COPY your Pay Now Service Key

#### Netcash Pay Now Callback

6. Choose the following for your Accept, Decline, Notify & Redirect URLs:

> http://domain.co.za/paynow/notify/

Issues & Feature Requests
-------------------------

We welcome your feedback.

Please contact Netcash Pay South Africa with any questions or issues.
