---
updated_at: 12/22/2016 11:18 AM
ms.date: 12/22/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/master/Azure%20AD%20Cmdlets/index.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/master/Azure%20AD%20Cmdlets/index.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/69a74d14b76e6c637fe3fc27adde96a181b165dc/Azure%20AD%20Cmdlets/index.md
ms.topic: conceptual
ms.technology: Azure PowerShell
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: carolz
open_to_public_contributors: True
ms.service: active-directory
---
# Azure Active Directory PowerShell

Azure Active Directory PowerShell is the most commonly used user interface for IT Pros to manage their Azure Active Directory. These cmdlets cover a broad range of functionality that provide capabilities to retrieve data from the directory, create new objects in the directory or change existing objects and configure the directory and its features.

There are two PowerShell modules. The newer AzureAD V2 module implements the Graph API in PowerShell en provides a wide range of capabilities. The old MSOnline module can still be used for functionality that is not yet available in the AzureAD module.
If you are developing new PowerShell scripts with Azure AD cmdlets we advise you to use the newer [Azure Active Directory PowerShell V2 cmdlets](https://docs.microsoft.com/en-us/powershell/azuread/v2/azureactivedirectory). We will begin deprecating the older MSOnline module when all of the functionality of that module has been migrated to the newer AzureAD module.

Please refer to the below detailed description of the modules for a full list of cmdlets and functionality.


Module | Description
------ | -----------
[AzureAD](https://docs.microsoft.com/en-us/powershell/azuread/v2/azureactivedirectory) | Azure Active Directory PowerShell v2
[MSOnline](https://docs.microsoft.com/en-us/powershell/msonline/v1/azureactivedirectory)| Azure Active Directory PowerShell v1

