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
