Creat an application from android studio integrated with SAP wizard.

1) Open android studio and choose "Start a new SAP Cloud Platform Android Project".
![image](images/1.png)

2) Once the wizard is open fill in the required fields as shown below and click next. 
![image](images/2.png)
![image](images/3.png)

3) On Cloud configuration tab, by default “use existing” tab is selected, make sure the application id “com.sap.android.sdk.demo” created in step2 of this document is selected from the drop down and click next. 
![image](images/4.png)

4) In the odata services tab, you will notice the sample service which was added as part of assigned features while creating the application in mobile services cockpit. Click next. 

5) On the android studio project tab provide the following configuration data and click next. 
![image](images/5.png)

6) On the projectc features tab, provide the following configuration data. 

    | Field | Value |
    | ------------- |-------------|
    | Use Discovery service as configuration provider | Uncheck |
    | Odata | Check |
    | Create a sample user experience for the selected odata destination | Check |
    | Enable Logging | Check |
    | Enable Upload | Check |
    | Enable Usage Reporting | Uncheck |
    | Enable Push | Check |

    ![image](images/6.png)

    1. When the Enable Push checkbox is checked, an error message is shown explaining that you need to specify a google-services.json file. We will obtain this file from the [Cloud Messaging](https://firebase.google.com/docs/cloud-messaging/) feature in [Google Firebase](https://firebase.google.com/).

    2. login using your gmail to firebase console. once logged in, click on "Go to console" on top right.
    ![image](images/15.png)

        click on "Add Project", give a project name and click continue. 
        ![image](images/16.png)

        In setp3 from the drop down select "Default Account for Firebase" and click create project

        Once the project is created, it opens the landing page of the project. Click on the android icon below the text “Get started by adding Firebase to your app”
        ![image](images/17.png)

        Fill android package name as "com.sap.android.sdk.demo" and App nickname(optional) as "androidSdkDemo" and click on Register app. 

        Click on "Download google-services.json" button in step 2 of "Add Firebase to your Android app" and click next.
        ![image](images/18.png)

        click next for step 3 and click "skip this setp" for step 4.
        
        Browse for the downloaded file "google-services.json" and upload it in push notificaiton
        ![image](images/19.png)

7) The project gets genereated and wait for the build to finish. 
![image](images/8.png)

8) Choose teh emulator for running the app.
    for more information on creating virutual Devices that run in the android emulator, see [here](https://developer.android.com/studio/run/managing-avds).
![image](images/9.png)

    Click the Run toolbar icon.

    ![image](images/10.png)

9) The Welcome screen is shown the first time the app is launches.

    ![image](images/11.png)

    Sign in with your credentails

    ![image](images/12.png)

    The passcode (or fingerprint if enabled) screen provides an additional layer of security for your app.

    ![image](images/13.png)

    The passcode policy can be modified in the mobile service cockpit under Client policies feature. 

    The first screen of the application shows all the entities that are present in sample odata service.

    ![image](images/14.png)
