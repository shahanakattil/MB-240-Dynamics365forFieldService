# Practice Lab 14 – Customer Voice

## Scenario

You are a dispatch manager at Relecloud who has been tasked with trying the Customer Voice functionality to capture feedback on work orders before rolling it out to your customers.

## Exercise 1: Create survey

In this exercise, you will create a project and use a template to create a survey.

### Task 1: Create project

1. Navigate to <https://customervoice.microsoft.com/Pages/ProjectPage.aspx>.

1. Sign in with your Dynamics 365 tenant credentials.

1. Create a new Project.

    ![](../images/custom-voice-01.png)

1. Select the **Service visit** template

1. Click **Next**

    ![](../images/custom-voice-02.png)

1. Select the **Prod-Env** Dynamics 365 environment. If the environment is not listed, click **See all environments**.

    ![](../images/custom-voice-03.png)

    ![](../images/custom-voice-04.png)

1. Click **Create**.

1. Click on **All Projects (1)**

1. Click on the ellipsis (2) next to your project and select **Rename (3)**.

1. Enter **Work Order Visit Feedback** and click on **Rename**.

    ![](../images/custom-voice-06.png)

    ![](../images/custom-voice07.png)

### Task 2: Customize survey

1. Select your project.

1. Click in the **Header** and change **Field service feedback** to **How did we do?**.

    ![](../images/custom-voice08.png)

1. Hover the mouse over the header and click on the **Theme color (1)** icon and change from 2266e3 to **ffdd66 (2)**.

    ![](../images/custom-voice-09.png)

1. Hover the mouse over the header and click on the **Image (1)** icon and choose one of the images (2) from the gallery.

    ![](../images/custom-voice10.png)

1. Select question 1 and set as **Required**.

1. Select question 2 and set as **Required**.

    ![](../images/custom-voice-11.png)

1. After the second question in the survey and click on **+ Add new** and click on the chevron(V) and select the **Net Promoter Score** question type. Set the question as **Required**.

    ![](../images/custom-voice-12.png)

    ![](../images/custom-voice-13.png)

    ![](../images/custom-voice-14.png)

1. Click on **Post-survey message** and change the Heading from *Thanks!* to **Thank you for your feedback** and change the Message to **We look at all feedback to improve our service.**

    ![](../images/custom-voice-15.png)

1. Click in the Footer and enter **The feedback you submit will not be shared outside of the company.**

    ![](../images/custom-voice-16.png)

1. Expand **Customization** and select **Personalization**.

    ![](../images/custom-voice-17.png)

1. Click + **Add variable** and enter **workordernumber** with default value **your booking**.

1. Click **Save**.

    ![](../images/custom-voice18.png)

1. Click **Close**.

1. Select **Formatting**

1. Toggle **Progress bar** to **Off** and close the formatting pane.

    ![](../images/custom-voice-19.png)

1. Click into the section header that starts with *Hi {{First Name}}* and clear the text, click on the **variables** drop-down and select **workordernumber**.

    ![](../images/custom-voice20.png)

    ![](../images/custom-voice-21.png)

1. Click **Preview**.

    ![](../images/custom-voice22.png)

1. Click **Back**.

    ![](../images/custom-voice-23.png)

### Task 3: Satisfaction metrics

1. Select your survey.

1. Expand **Customization** and select **Satisfaction metrics**

1. Click **+ Add metric**

1. Select **Net Promoter Score** and select the third question.

    ![](../images/custom-voice-24.png)

1. Click **Save**.

    ![](../images/custom-voice-25.png)

1. Click **Cancel**

## Exercise 2: Send survey

In this exercise, you will create an email template and send the survey by email.

### Task 1: Configure email template

1. Navigate to <https://customervoice.microsoft.com>

1. Select your project.

1. Select your survey.

1. Click on the **Send** tab.

1. Click on the **Email** tile.

    ![](../images/custom-voice26.png)

1. Click on the **Template** drop-down and select **Create new**.

    ![](../images/custom-voice-27.png)

1. Enter **Field Service Visit** and click **Add**.

    ![](../images/custom-voice28.png)

1. Click on the **Template** drop-down and **Field Service Visit**.

    ![](../images/custom-voice29.png)

1. Click in the top of the body of the email template.

1. Click on the **Insert** drop-down and select **First question of the survey (1)**.

1. Replace the subject line with **Please provide feedback on**, click on the **Insert** drop-down and select **Personalized variables** and then select **workordernumber (2)**.

1. Click **Save (3)**

    ![](../images/custom-voice30.png)

1. Click **Cancel (4)**

### Task 2: Send the survey

1. Click on the **Send** tab.

2. Click on the **Email** tile.

3. Click on the **Template** drop-down and select the **Field Service Visit** template you created.

4. Click in the Recipients field and enter **customer@contosot.com**.

    ![](../images/sendmail.png)

5. Click **Send**

## Exercise 3: Send survey when a work order is completed

In this exercise, you will use Power Automate to send a survey when a work order is completed.

### Task 1: Configure automation

1. Navigate to <https://customervoice.microsoft.com>

1. Select your project.

1. Select your survey.

1. Click on the **Send** tab, and select **Resend** drop-down.

1. Click **Automate**.

    ![](../images/custom-voice32.png)

1. Select your region on the pop up and select get started. Now select **Send a survey when a work order is completed or closed in Dynamics 365** template. You may need to click on **See more templates**.

    ![](../images/custom-voice33.png)

    ![](../images/custom-voice34.png)

1. Select **Sign in** on both the connections and enter any necessary details when prompted.

    ![](../images/custom-voice-35.png)

    ![](../images/custom-voice-36.png)

1. Click **Continue**.

1. Expand the steps in the flow and select your **Prod-Env** for all the flows.

    ![](../images/custom-voice-38.png)

1. Now, select the send a survey step.

1. Clear the **Email** template field and select the **Field Service Visit** template you created.

    ![](../images/custom-voice37.png)

1. Click **Save**.

    ![](../images/custom-voice-40.png)
    
 **Result:** You have successfully created a project and using a template, created a survey. Followed by creating an email template. Finally sending the survey using the email template. 
