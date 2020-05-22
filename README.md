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

## Contents


| File/folder       | Description                                |
|-------------------|--------------------------------------------|
| `templates/AutoApproveRequests/AutoApproveOfferShiftRequests.zip`  | Allows a team manager to automatically approve Offer Shift requests  |

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
    - Under "Review Package Content" > Related resources
        - Click on "Select during import" and select the account you want to use
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
