---
published: false                        # Optional. Set to true to publish the workshop (default: false)
type: workshop                          # Required.
title: Copilot Studio Lab              # Required. Full title of the workshop
short_title: Copilot studio lab     # Optional. Short title displayed in the header
description: This is a workshop for...  # Required.
level: beginner                         # Required. Can be 'beginner', 'intermediate' or 'advanced'
authors:                                # Required. You can add as many authors as needed      
  - Sidali KADOUCHE
  - Melissa SARI
contacts:                               # Required. Must match the number of authors
  - Author's email, Twitter...
duration_minutes: 20                    # Required. Estimated duration in minutes
tags: javascript, api, node.js          # Required. Tags for filtering and searching
#banner_url: assets/banner.jpg           # Optional. Should be a 1280x640px image
#video_url: https://youtube.com/link     # Optional. Link to a video of the workshop
#audience: students                      # Optional. Audience of the workshop (students, pro devs, etc.)
#wt_id: <cxa_tracking_id>                # Optional. Set advocacy tracking code for supported links
#oc_id: <marketing_tracking_id>          # Optional. Set marketing tracking code for supported links
#navigation_levels: 2                    # Optional. Number of levels displayed in the side menu (default: 2)
#sections_title:                         # Optional. Override titles for each section to be displayed in the side bar
#   - Section 1 title
#   - Section 2 title
---

# Build, deploy a Copilot using the Power Platform AI Capabilities and Azure   

During this hands on lab workshop you will learn how to create an intelligent solution using the power platform capabilities including copilot studio, AI Builder and how to interact with backend services like azure functions.

---
## Workshop Objectives
- Build and Deploy a backend API using Azure functions 
- Build and Deploy your custom Copilot using Copilot studio and Power platform capabilities
## Prerequisites
| | | |
|---------------|-----------------|-----------------|
| Git | https://git-scm.com |Optionnal|
| A code editor | https://aka.ms/get-vscode |Optionnal|
| Azure function vscode extension | https://marketplace.visualstudio.com/items?itemName=ms-azuretools.vscode-azurefunctions | Optionnal|
| A chromium-based browser | https://www.microsoft.com/edge | Requiered|

---

## Clone and deploy the azure function (Optional)

### Create the function resource on Azure portal
1. Open Azure portal: [portal.azure.com](https://portal.azure.com/#create/Microsoft.FunctionApp)

2. Select your resource group `user n` where n is your user number ex: `user 1

3. Enter a name and choose a region

4. Keep the deploy option as `Code`

5. In **Runtime Stack**, choose the `.NET` build preset

6. For the **Version**, enter `8 (LTS)`

7. For the **Operating system**, keep `Windows`

8. Click **Hosting options and plans**, Keep `Consumption plan` and click **Create new**

9. Click on **Create**

### Clone the function code repository
Open a terminal in a new folder and run the following command to clone the repository

```sh
git clone https://github.com/sidkadouc/hybridcode_bookingfunction.git
```
open the new cloned repository in vs editor

### Deploy the function code to azure
1. Open the bookingfunction folder in vs code

2. Type `CTRL` + `SHIFT` + `P` to open the command palette

3. Type `Azure Functions: Deploy to Function App` and press `Enter`

4. Select the folder that contains the function code

5. Select the function you've created before and confirm the deployment

