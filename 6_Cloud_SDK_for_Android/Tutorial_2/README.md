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

    ![image](images/6.png)
    ![image](images/7.png)

7) Click finish on the project features tab. The project gets genereated and wait for the build to finish. 
![image](images/8.png)

8) Choose teh emulator for running the app.
    for more information on creating virutual Devices that run in the android emulator, see [here](https://developer.android.com/studio/run/managing-avds).
![image](images/9.png)

    Click the Run toolbar icon.

    ![image](images/10..png)

9) The Welcome screen is shown the first time the app is launches.

    ![image](images/11.png)

    Sign in with your credentails

    ![image](images/12.png)

    The passcode (or fingerprint if enabled) screen provides an additional layer of security for your app.

    ![image](images/13.png)

    The passcode policy can be modified in the mobile service cockpit under Client policies feature. 

    The first screen of the application shows all the entities that are present in sample odata service.

    ![image](images/14.png)
