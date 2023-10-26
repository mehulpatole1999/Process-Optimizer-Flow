# Process-Optimizer-Flow
Create a Power Automate Flow to improve the process and save time.
Title: Designing a Power Automate Flow to Extract and Convert Zip Files from Outlook to OneDrive

Abstract:
This whitepaper provides a comprehensive guide on designing a Power Automate flow for beginners, focusing on extracting zip files from a shared mailbox in Outlook, storing them in a OneDrive folder, and converting the zip files into XLSX files in another OneDrive folder. We will break down each step, from creating the flow to testing it.

Table of Contents:
1. Introduction
2. Prerequisites
3. Designing the Power Automate Flow
   3.1. Creating the Flow
   3.2. Trigger Configuration
   3.3. Storing Zip Files from Outlook in OneDrive
   3.4. Extracting Zip Files from OneDrive
   3.5. Converting Zip Files to XLSX
   3.6. Storing XLSX Files in OneDrive
   3.7. Post message in a teams chat or channel
4. Testing and Troubleshooting
5. Conclusion

1. Introduction:
Power Automate is a powerful automation tool by Microsoft that enables you to create workflows to automate various tasks. In this guide, we will focus on creating a flow to automate the process of extracting zip files from a shared mailbox in Outlook and converting them into XLSX files, all while utilizing OneDrive for storage.

2. Prerequisites:
   - A Microsoft 365 subscription.
   - Access to Power Automate and OneDrive.
   - Permission to access the shared mailbox in Outlook.

3. Designing the Power Automate Flow:

3.1. Creating the Flow:
   - Log in to Power Automate.
   - Click on "Create" and select "Automated cloud flow"

3.2. Trigger Configuration:
   - Choose the trigger that initiates the flow. In this case, select "Outlook - When a new email arrives in a shared mailbox."

3.3. Storing Zip Files from Outlook in OneDrive:
   -Add "Apply to Each" loop for processing multiple files.
   - Add a "Create file" action for OneDrive.
   - Configure the action to create a file in your chosen OneDrive folder and use the extracted zip file as the content.

3.4. Extracting Zip Files from OneDrive:
   - In the trigger, specify the shared mailbox's email address.
   - Add a condition to check if the email contains zip files.
   - Use "Extract archive to folder" action to convert the zip files and store it on OneDrive at specific path, Else "Do nothing".

3.5. Converting Zip Files to XLSX:
   - Inside the loop, use an "Extract archive" action to unzip the files.
   - If needed, add a condition to filter only specific files.
   - Use appropriate connectors or custom code to convert the files to XLSX format.

3.6. Storing XLSX Files in OneDrive:
   - Add another "Create file" action for OneDrive.
   - Configure it to create XLSX files in a different OneDrive folder.

3.7. Post a message in a teams chat or channel:
-Add an action to post a message in team
chat for final confirmation that our flow has ran successfully

4. Testing and Troubleshooting:
   - Test the flow with sample emails and zip files.
   - Monitor the flow's run history for any errors.
   - Troubleshoot issues by checking the detailed error messages and adjusting the flow accordingly.

5. Conclusion:
In this whitepaper, we've outlined the step-by-step process of designing a Power Automate flow for extracting zip files from a shared mailbox in Outlook, storing them in OneDrive, and converting them into XLSX files in another OneDrive folder. With this guide, beginners can efficiently automate this workflow, saving time and effort in handling attachments and file conversions.

By following these detailed instructions and experimenting with different settings, users can customize this flow to suit their specific needs, all within the user-friendly environment of Power Automate.
