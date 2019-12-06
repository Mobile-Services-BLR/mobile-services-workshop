# Read me for the Setup.

1) Get a Free Trial Account on SAP Clout Platform.

    1. If you do not have an SAP account, visit https://www.sap.com and click the Log On icon in the upper-right corner.
    ![image](images/1.png), if you already have an step2.

    2. Fill in the required fields and click submit.
    ![image](images/2.png)

    3. You will get a message that an activation link has been sent to you.
    ![image](images/3.png)

    4. Check your emails to find the activation button Click to activate your account.
    ![image](images/4.png)

    5. After activating your account, you will see the following screen.
    ![image](images/5.png)

2) Log on to SAP Cloud Platform.

    1. After activation, or if you already had an SAP account, go to the [SAP Cloud Platform Trial page](https://account.hanatrial.ondemand.com/) and click Log On.
    You will see an dialog to confirm the terms and condition for the SAP Cloud Platform Developer Edition. Check the check boxes and click Accept. This simply adds the SAP.com registration to your login account on SAP Cloud Identity. There is no cost associated with this upgrade.
    ![image](images/6.png)

    2. You will see a message that you need to verify your account with a phone number. Click Verify your phone number to trigger that flow.
    ![image](images/7.png)

    3. Enter your phone number and click New Code to retrieve a code. Please enter this code as well and click Continue to verify your account. After the verification, you will be logged off automatically.
    ![image](images/8.png)

    4. Click on Log on to log on to your verified account.
    ![image](images/9.png)

    5. Here, you can now create a subaccount which lives in a geographic region. Choose one of regions from this list.
    We suggest the Europe (Frankfurt) region because it has the largest list of services. If you want to use a region closer to you, [check to be certain it has the services you want before selecting it](https://help.sap.com/doc/aa1ccd10da6c4337aa737df2ead1855b/Cloud/en-US/3b642f68227b4b1398d2ce1a5351389a.html?3b642f68227b4b1398d2ce1a5351389a.html).
    ![image](images/10.png)

    6. You will then see a dialog box while the account is set up. When complete, the dialog box will look like this. Click Continue to close to popup.
    ![image](images/11.png)

3) Navigate to Cloud Foundry Space

    1. You will see two buttons on the welcome screen of the SAP Cloud Platform Cockpit. Click on Enter Your Trial Account to see your global account.
    ![image](images/12.png)

    2. The global trial account contains one subaccount and space. Navigate to subaccount by clicking on the tile named trial (this name may vary if you created the subaccount manually).
    ![image](images/13.png)

    3. To get to the space, in which your applications and services live, click on the dev space.
    ![image](images/14.png)

    4. On the cloud foundry space, expand services on the navigation view and click on service market place
    ![image](images/15.png)

    5. Search for mobile in the search window and click on mobile services as shown in below snapshot.
    ![image](images/16.png)

4) Mobile Services Cockpit.

    1. In the mobile services overivew page, click on support.
    ![image](images/17.png)
    This will open a new tab with mobile services tenant which will promt you to select organization and space. By default there is only one organization and space. if you have additional acocunts select the appropriate account and click open.
    ![image](images/18.png)

    2. On the mobile servcies tab at the bottom left click on important links.
    ![image](images/19.png) 
    This will load some of the links required for mobile services, copy 2 urls "copy Admin API" and "copy Admin UI" into a notepad for further reference. 
    ![image](images/20.png)

5) Enable SAP Web IDE full-Stack. 

    1. Switch back to sap cloud paltform cockpit homepage. 
    ![image](images/21.png)
    click on the 1st tab on the breadcrum as shown in the below snapshot.
    ![image](images/22.png)
    On the homepage, scroll down to "Enviroment" tab and click on  "Access Neo Trial" as shown below.
    ![image](images/23.png)

    2. Now in the neo environment, expand connectivity under navigation view and select destinations
    ![image](images/28.png)
    click on new destination and fill in the fields mentioned below and click save.

        ![image](images/29.png)

        | Field | Value |
        | ------------- |-------------|
        | Name | MobileServiceCF |
        | Type | HTTP|
        | URL | (paste the url "Copy Admin API" from mobile services cockpit)
        | Proxy Type | Internet |
        | Authentication | BasicAuthentication |
        | User name | (enter the email id used to access cloud platform)
        | passord | (enter the password)|

        Additional properties value
        
        | Field | Value |
        | ------------- |-------------|
        | HandleRedirects | false |
        | SkipSSOTokenGenerationWhenNoUser | true |
        | WebIDEEnabled | true |
        | WebIDEUsage | mobile |

    3. In the service catalog, search for Web IDE and select the SAP Web IDE Full-Stack service.
    ![image](images/25.png)
    Once the service page loads, enable the service. This may take few minutes.
    ![image](images/26.png)
    Once the service is enabled, click Go to Service. this opens full stack SAP Web IDE.
    ![image](images/27.png)

6. Setup Webide to link cloud found mobile services.

    1. Open Preferences window by clicking on the gear icon and click Extensions
    ![image](images/30.png)

         Search with mobile to find required extension Mobile Services App Development Tools, toggle it to ON and choose Save.
         This extension is used for creating and developing Mobile development kit and SAP Mobile Cards based applications along with creating backend OData service (from Scratch) that provides capabilities enabling you to quickly build an mobile enabled OData service that constitutes your mobile back-end service for mobile applications.
        ![image](images/31.png)

    2. In the preferences window select "Cloud Foundry", under cloud foundry space if you have only 1 account which was created during this execrise, leave the default values and click save. if you have more than one organization select the values.
    ![image](images/32.png)

7. Refersh your webide once, before you start the development.