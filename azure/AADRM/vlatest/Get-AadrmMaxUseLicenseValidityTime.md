---
external help file: Microsoft.RightsManagementServices.Online.Admin.PowerShell.dll-Help.xml
online version: http://go.microsoft.com/fwlink/?LinkID=529558
schema: 2.0.0
ms.assetid: CDD8C715-6C63-40BC-AF75-F842FDFD5E62
updated_at: 2/8/2017 6:01 PM
ms.date: 2/8/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/master/Azure%20Information%20Protection/AADRM/vlatest/Get-AadrmMaxUseLicenseValidityTime.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/master/Azure%20Information%20Protection/AADRM/vlatest/Get-AadrmMaxUseLicenseValidityTime.md
gitcommit: https://github.com/Azure/azure-docs-powershell-aip/blob/b5b814c02caa6cd576a3db614749957f10782144/Azure%20Information%20Protection/AADRM/vlatest/Get-AadrmMaxUseLicenseValidityTime.md
ms.topic: reference
ms.prod: powershell
ms.technology: Azure Powershell
author: cabailey
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: cabailey
open_to_public_contributors: False
ms.service: rights-management
---

# Get-AadrmMaxUseLicenseValidityTime

## SYNOPSIS
Gets the maximum validity time for Rights Management use licenses.

## SYNTAX

```
Get-AadrmMaxUseLicenseValidityTime [<CommonParameters>]
```

## DESCRIPTION
The **Get-AadrmMaxUseLicenseValidityTime** cmdlet gets the maximum validity time, in days, for Azure Rights Management use licenses in your organization. The default value is 30 days.

## EXAMPLES

### Example 1: Get the maximum validity time
```
PS C:\>Get-AadrmMaxUseLicenseValidityTime
30
```

This command gets the maximum validity time for use licenses in your organization.

## PARAMETERS

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Set-AadrmMaxUseLicenseValidityTime](xref:AADRM/vlatest/Set-AadrmMaxUseLicenseValidityTime.md)


