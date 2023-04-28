# Practice Lab 10 - Field Service mobile app

## Exercise 1 – Configure Field Service mobile app for frontline workers

In this exercise you will configure settings for work orders including priorities and resolutions.

   >Note: The **[DeploymentId]/[DID] can be found under the environment details tab in the user name (example: `odl_user_xxxxxx.onmicrosoft.com`) **xxxxxx** is the [DeploymentID]**.

### Task 1 – Configure security and offline profile

1. In the **Dynamics 365 Field Service app**, click **Get Started** from My work panel.

1. Under Set up your frontline workers, click **Set up**.

    ![](../images/Set-up-1.png)

1. Select your user for **Users**.

1. Select your **Time Zone**.

1. Click **Save and Close**.

    ![](../images/Set-up-2.png)

### Task 2 – Create work order

1. In the **Dynamics 365 Field Service app**, click the **Service** area in the bottom-left of the sitemap, and in the **Scheduling** group select **Work Orders**.

1. Click **+ New**.

    ![](../images/Set-up-3.png)

1. Select the **odl_user_DID_Relecloud** account you created in an earlier lab for **Service Account**.

1. Select the **odl_user_DID_Service_Printer** incident type you created in a previous lab for **Primary Incident Type**.

1. Select the **Settings** tab.

    ![](../images/Set-up-4.png)

1. Select the **odl_user_DID_Normal** priority you created in a previous lab for **Priority**.

1. Click **Save**.

    ![](../images/Set-up-5.png)

1. In the **Dynamics 365 Field Service app**, click the **Service** area in the bottom-left of the sitemap, and in the **Scheduling** group select **Schedule Board**.

1. Select the  **odl_user_DID_Board** tab.

1. Drag the requirement for the work order to an available slot for today or tomorrow for your resource.

    ![](../images/Set-up-6.png)

### Task 3 – Install the mobile app

1. In your mobile devices app store, search for **Field Service Dynamics 365**.

1. Select the **Field Service (Dynamics 365)** app and install.

1. Open the app.

1. Tap **Sign in** and log in with your Dynamics 365 tenant credentials.

1. Verify that you can see the booking you made in Task 2.

### Task 4 – Process the booking

1. Tap to open the booking.

1. Change **Booking Status** to **Traveling** and tap **Save**. The color of the booking on the schedule board will change.

    ![](../images/Install-the-mobile-app-2.jpg)

1. Change **Booking Status** to **In Progress** and tap **Save**. The color of the booking on the schedule board will change.

1. Tap the **Customer** tab.

1. Tap **Get Directions**.

    ![](../images/Install-the-mobile-app-7.jpg)

1. Close the mapping app.

1. Tap the **Service** tab.

1. Check the **Clean Printer Assembly** task.

1. Check the **Replace Toner** task.

1. Check the **Final Test** task.

1. Tap to open the **Inspect Printer** task.

    ![](../images/Install-the-mobile-app-9.jpg)

1. If you have barcode available click on the barcode symbol and allow the app to use your device and scan a barcode.

1. If you do not have a barcode, enter **ABC888** for **Serial number**.

1. Select **Good** from the **Condition** drop-down field.

1. Enter **500** for **Page Count**.

    ![](../images/Install-the-mobile-app-10.jpg)

1. Enter **All ok** for **Comments**.

1. Tap on **Photo** and allow the app to use your camera and take a photo.

1. Slide **% Complete** to **100**.

1. Select **Pass** for **Result**.

1. Set **Actual Duration** to **15 minutes**.

1. Tap **Save**.

    ![](../images/Install-the-mobile-app-14.jpg)

1. Tap **<** to return to the booking.

1. Tap to open the **Printer Service Fee** service.

1. Tap **Used** for **Line Status**.

1. Tap **Save**.

    ![](../images/Install-the-mobile-app-13.jpg)

1. Tap **<** to return to the booking.

1. Tap to open the **Remote Printer** product.

1. Tap **Used** for **Line Status**.

1. If a popup message appears that says you do not have quantity on hand, click **OK**.

1. Tap **Save**.

    ![](../images/Install-the-mobile-app-12.jpg)

1. Tap **<** to return to the booking.

1. Tap the **General** tab.

1. Change **Booking Status** to **Completed** and tap **Save**.

1. Tap **<** to return to the agenda.
