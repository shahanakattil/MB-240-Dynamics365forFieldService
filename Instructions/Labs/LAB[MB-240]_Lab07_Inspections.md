# Practice Lab 7 - Inspections

## Exercise 1 - Create and use an Inspection Template

In this exercise, you will be defining an inspection template and adding it to a server type task.

### Task 1 - Create Inspection Template

1. In the **Dynamics 365 Field Service app**, click the **Resources (1)** area in the bottom-left of the sitemap, and select **Settings (2)** from the list. 

    ![](../images/settings-select.png)

1. In the **Work Orders** group select **Inspection Templates (1)**.

1. Click **+ New (2)**.

    ![](../images/inspection-01.png)

1. Enter **PrinterInspection** for **Name for Inspection (1)**.

1. Click on **TextBox (2)** to add question.

1. Enter **Serial number** for **Question1 (3)** title.

1. Toggle **Required (4)** to On.

1. Click **Advanced (5)**.

    ![](../images/28.png)

1. Select **Barcode** for **Input type**.

    ![](../images/inspection-03.png)

1. Select **Toolbox (1)** tab.

1. Click on **Dropdown (2)** to add question.

1. Enter **Condition (3)** for **Question2** title.

1. Toggle **Required (4)** to On.

1. Change **Item 1** to **Poor (5)**.

1. Change **Item 2** to **Satisfactory (5)**.

1. Change **Item 3** to **Good (5)**.

    ![](../images/inspection-04.png)

1. Click on **Number (1)** to add question.

1. Enter **Page Count (2)** for **Question3** title.

1. Select the **Advanced (3)** tab.

    ![](../images/inspection-05.png)

1. Toggle **Whole Number** to On.

    ![](../images/inspection-06.png)

1. Select the **Toolbox** tab.

1. Click on **TextBox (1)** to add question.

1. Enter **Comments (2)** for **Question4** title.

1. Select the **Advanced (3)** tab.

    ![](../images/29.png)

1. Select **Multiline** for the **Input type** drop-down.

    ![](../images/inspection-08.png)

1. Select the **Toolbox** tab.

1. Click on **File (1)** to add question.

1. Enter **Image** for **Question5 (2)** title.

1. Click the **Preview (3)** tab.

    ![](../images/30.png)

1. Click **Save**.

1. Click **Publish** and click **Publish** again.

    ![](../images/31.png)

> **Congratulations** on completing the task! Now, it's time to validate it. Here are the steps:
> - Select the **Lab Validation** tab located at the upper right corner of the lab guide section.
> - Hit the Validate button for the corresponding task. If you receive a success message, you can proceed to the next task. 
> - If not, carefully read the error message and retry the step, following the instructions in the lab guide.
> - If you need any assistance, please contact us at labs-support@spektrasystems.com. We are available 24/7 to help you out.

### Task 2 - Add Inspection Template to Service Type Task

1. In the **Work Orders** group select **Service Task Types**.

    ![](../images/service-task-03.png)

1. Click **+ New**.

1. Enter **InspectPrinter** for **Name (1)**.

1. Enter **5 Minutes** for **Estimated Duration (2)**.

1. Toggle **Has Inspection (3)** to **Yes**.

1. Select the **PrinterInspection** inspection template you created in Task 1 for **Inspection Template (4)**.

1. Click **Save (5)**.

   ![](../images/32.png)

1. In the **Work Orders** group select **Incident Types**.

1. Edit the **ServicePrinter** incident type.

    ![](../images/33.png)

1. Select the **Service Tasks** tab.

1. Click **+ New Incident Type Service Task**.

    ![](../images/34.png)

1. Enter **InspectPrinter** for **Name (1)**.

1. Select the **InspectPrinter** service task type you created in Task 2 for **Task Type (2)**.

1. Click **Save and Close (3)**.

    ![](../images/35.png)

1. Click **Save & Close**.

### Task 3 – Download an image

1. In the browser, open Microsoft Bing and do an image search for printers.

1. Right-click on the image of the printer and select **Save image as** and click **Save**.

### Task 4 – Create a new Work Order and view the inspection

1. In the **Dynamics 365 Field Service app**, click the **Settings (1)** area in the bottom-left of the sitemap, and select **Service (2)** from the list. 

    ![](../images/inspection-14.png)

1. In the **Scheduling** group select **Work Orders**.

1. Click **+ New**.

    ![](../images/36.png)

1. Select the **Relecloud** account you created in Task 1 for **Service Account**.

1. Select the **ServicePrinter** incident type you created in a previous lab for **Primary Incident Type**.

    ![](../images/37.png)

1. Click **Save**.

1. Wait about 30 seconds to a minute and click **Refresh** in the command bar.

1. Select the **Service Tasks** tab and verify that the four tasks were added.

    ![](../images/38.png)

1. Open the **InspectPrinter** work order service task.

1. Enter **122333** for **Serial number (1)**.

1. Select **Satisfactory** from the **Condition (2)** drop-down field.

1. Enter **999** for **Page Count (3)**.

1. Enter **No problems found** for **Comments (4)**.

1. Click on **Choose file(s)** and browse to the image you downloaded in Task 3 and click **Open (5)**.

1. Click **Save (6)**.

    ![](../images/39.png)

1. Select **Pass** for **Result (1)**.

1. Click **Mark Complete (2)**.

    ![](../images/40.png)

> **Congratulations** on completing the task! Now, it's time to validate it. Here are the steps:
> - Select the **Lab Validation** tab located at the upper right corner of the lab guide section.
> - Hit the Validate button for the corresponding task. If you receive a success message, you can proceed to the next task. 
> - If not, carefully read the error message and retry the step, following the instructions in the lab guide.
> - If you need any assistance, please contact us at labs-support@spektrasystems.com. We are available 24/7 to help you out.

**Result:** You have successfully definied an inspection template by adding it to a service type task. Also you were able to view inspection by creating a work order.
