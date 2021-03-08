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

## Power Automate Templates

The Power Automate/Flow Templates templates are now available officially: https://flow.microsoft.com/en-us/connectors/shared_shifts/shifts-for-microsoft-teams/

## PowerBI Templates

**PowerBI Template Properties (filter by date/group):**

Page One:
Hours worked by userid/name
Open shifts count by day and group name
All shifts count / Open shifts count / Number of groups

Page Two:
Open shifts count by datetime and group name
All shifts count by datetime and group name
All shifts count / Open shifts count / Number of groups / Longest Shift / Shortest Shift / Average Shift / Longest open Shift / Shortest Open Shift / Average Open Shift

Page Three:
Open Hours Worked by datetime and group name
Hours worked by datetime and group name
All shifts count / Open shifts count / Number of groups / Longest Shift / Shortest Shift / Average Shift / Longest open Shift / Shortest Open Shift / Average Open Shift

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
