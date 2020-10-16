---
page_type: sample
languages:
- json
products:
- Shifts
- Microsoft Teams
- Power Automate
description: "Power Automate templates that enable you to automate operations in Microsoft Teams Shifts"
urlFragment: "Microsoft-Teams-Shifts-Power-Automate-Templates"
---

# Power Automate Templates for the Shifts app in Microsoft Teams

<!-- 
Guidelines on README format: https://review.docs.microsoft.com/help/onboard/admin/samples/concepts/readme-template?branch=master

Guidance on onboarding samples to docs.microsoft.com/samples: https://review.docs.microsoft.com/help/onboard/admin/samples/process/onboarding?branch=master

Taxonomies for products and languages: https://review.docs.microsoft.com/new-hope/information-architecture/metadata/taxonomies?branch=master
-->

This template collection is to help you create Flows in Power Automate to automate several scenarios.

## Templates

1. [Auto Approve Offer Shift Requests](#Auto-Approve-Offer-Shift-Requests)
2. [Auto Approve Open Shift Requests](#Auto-Approve-Open-Shift-Requests)
3. [Auto Approve Swap Shifts Requests and Send Email Notification](#Auto-Approve-Swap-Shifts-Requests-and-Send-Email-Notification)
4. [Auto Convert Shift to Open Shift](#Auto-Convert-Shift-to-Open-Shift)
5. [Share My Shifts as iCalendar Feed](#Share-My-Shifts-as-iCalendar-Feed)

### Auto Approve Offer Shift Requests
Allows a team manager to automatically approve Offer Shift requests in the team.

> When one team member offers a shift to another member, and the request is accepted by that member. It it then sent to the team manager for approval. With this flow setup to run by a team manager, it'll automatically approve any offer shift requests the manager receives.

Template: [`templates/AutoApproveRequests/AutoApproveOfferShiftRequests.zip`](/templates/AutoApproveRequests/AutoApproveOfferShiftRequests.zip) 
[See template import instructions](#Using-the-templates)
![Auto Approve Offer Shift Request](/images/AutoApproveOfferShiftRequest.png)

### Auto Approve Open Shift Requests
Allows a team manager to automatically approve Open Shift requests in the team.

> When a team member requests an open shift, the request is sent to the team manager for approval. With this flow setup to run by a team manager, it'll automatically approve any open shift requests the manager receives.

Template: [`templates/AutoApproveRequests/AutoApproveOpenShiftRequest.zip`](/templates/AutoApproveRequests/AutoApproveOpenShiftRequest.zip) 
[See template import instructions](#Using-the-templates)
![Auto Approve Open Shift Request](/images/AutoApproveOpenShiftRequest.png)

### Auto Approve Swap Shifts Requests and Send Email Notification
Allows a team manager to automatically approve Swap Shift requests in the team and send an email notifying the affected team members.

> When one team member sends a request to swap shifts to another member, and the request is accepted by that member. It it then sent to the team manager for approval. With this flow setup to run by a team manager, it'll automatically approve any swap shifts requests the manager receives. It will also send an email notification to both members notifying them that the request was approved.

Template: [`templates/AutoApproveRequests/AutoAcceptSwapRequestsandEmailNotify.zip`](/templates/AutoApproveRequests/AutoAcceptSwapRequestsandEmailNotify.zip) 
[See template import instructions](#Using-the-templates)
![Auto Approve Offer Shift Request](/images/AutoApproveSwapShiftsRequestAndEmail.png)

### Auto Convert Shift to Open Shift
Allows a team manager to automatically approve the process of converting a Shift into an Open Shift.

> The team member should offer the shift they want to return back to the team manager. With this flow setup to run by a team manager, it'll automatically search for any matching open shifts (with the same start time, end time, theme and group). If a matching Open Shift is found, the slot count is incremented; otherwise a new Open Shift is created from the information in the Shift.

Template: [`templates/AutoApproveRequests/AutoConvertShiftToOpenShift.zip`](/templates/AutoApproveRequests/AutoConvertShiftToOpenShift.zip) 
[See template import instructions](#Using-the-templates)
![Auto Convert Shift to Open Shift](/images/AutoConvertShiftToOpenShift.png)

### Share My Shifts as iCalendar Feed
Allows a user to publish their shifts as an [Internet Calendar](https://en.wikipedia.org/wiki/ICalendar), so they can view their shifts schedule in Outlook or their mobile device calendars

> After importing the template into a new Flow, copy the iCalendar feed URL from the "When a HTTP request is received" action:
![screenshot](/images/iCalendarFeedLink.png)
>This URL can then be added as a subscription into most calendar applications like [Outlook](https://support.microsoft.com/en-us/office/import-or-subscribe-to-a-calendar-in-outlook-on-the-web-503ffaf6-7b86-44fe-8dd6-8099d95f38df) and natively on your iOS/Android devices. 
![screenshot](/images/AddCalendarFromInternet.png)
>Your calendar app should poll this Flow every hour and automatically get updates to your schedule.

Template: [`templates/Calendar/ShareMyShiftsasiCalendarFeed.zip`](/templates/Calendar/ShareMyShiftsasiCalendarFeed.zip) 
[See template import instructions](#Using-the-templates)
![Auto Convert Shift to Open Shift](/images/ShareMyShiftsAsICalendarFeed.png)

## Prerequisites

Create your team in the Shifts app in [Microsoft Teams](https://teams.microsoft.com).


## Using the templates

- Login to [Power Automate](https://flow.microsoft.com/)
- Navigate to the Flow import:
    - Click on the "My Flows" tab on the left navigation menu
    - Click on the "Import" button in the top command bar
- Import the package:
    - Click on the "Upload" button to select the template zip file
    - Wait for it to upload
    - Under "Review Package Content" > Import Options
        - Choose to "Create as new" Flow
    - Under "Review Package Content" > "Related resources"
        - Click on "Select during import" to select the account connection to use with each resource type.
        - If you don't have an existing connection to the resource type, create a new connection to the resources that the Flow uses. 
        - The resource types should be listed during the import, and can include
            - Microsoft Teams (The account you use to sign in here, typically has to be a owner/manager of the team)
            - Office 365 Users
            - Office 365 Outlook
    - Click the "Import" button
- Configure the imported Flow:
    - Navigate to the new Flow that was imported
    - Select the Team that you want the Flow to operate on (do this for all actions where a Team is referenced)
    - Save the Flow

## PowerBI Templates

**PowerBI Dashboard with Display Name:**

Template: [`/PowerBI/Shifts%20Template%20with%20UserName.pbit`](/PowerBI/Shifts%20Template%20with%20UserName.pbit) 

1. Download excel doc (save to onedrive or a location flow can access), Flow template, PowerBI template
2. Navigate to [https://flow.microsoft.com/](https://flow.microsoft.com/)
3. Import flow template and edit it 
![Alt](/PowerBI/images/importbtn.png?raw=true)
4. On editing the uploaded flow
  * Select a team you would like reporting on
  * Update location/library/file/table to the location of the excel doc
  * Save and Run the flow.
  * Download the file when the flow completes and place it in a location for later. (NOTE: Using CTRL + Shift and right clicking will give you the open to copy the file path for later use.)
  
![Alt2](PowerBI/images/updateflowfields.png?raw=true)

5. Open the PowerBI template and enter the TeamID (not the name), StartDateTime, EndDateTime (ex: 2020-05-01T00:00:00.000Z), ExcellFileLocation
6. Click load

**PowerBI Dashboard without Display Name:**

Template: [`/PowerBI/Shifts%20Template.pbit`](/PowerBI/Shifts%20Template.pbit) 

1. Open the PowerBI template and enter the TeamID (not the name), StartDateTime, EndDateTime (ex: 2020-05-01T00:00:00.000Z)
2. Click load


## Contributing

This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.

When you submit a pull request, a CLA bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
