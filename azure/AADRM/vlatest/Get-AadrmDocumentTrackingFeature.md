---
external help file: Microsoft.RightsManagementServices.Online.Admin.PowerShell.dll-Help.xml
online version: http://go.microsoft.com/fwlink/?LinkId=623037
schema: 2.0.0
ms.assetid: 3F0BC472-41CC-41CA-A1B5-ACB84B1C2DA9
updated_at: 2/8/2017 6:01 PM
ms.date: 2/8/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/live/Azure%20Information%20Protection/AADRM/vlatest/Get-AadrmDocumentTrackingFeature.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/live/Azure%20Information%20Protection/AADRM/vlatest/Get-AadrmDocumentTrackingFeature.md
gitcommit: https://github.com/Azure/azure-docs-powershell-aip/blob/b5b814c02caa6cd576a3db614749957f10782144/Azure%20Information%20Protection/AADRM/vlatest/Get-AadrmDocumentTrackingFeature.md
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

# Get-AadrmDocumentTrackingFeature

## SYNOPSIS
Indicates whether document tracking is enabled or disabled for Azure Information Protection.

## SYNTAX

```
Get-AadrmDocumentTrackingFeature [<CommonParameters>]
```

## DESCRIPTION
The **Get-AadrmDocumentTrackingFeature** cmdlet indicates whether the Azure Information Protection document tracking feature is enabled or disabled.

## EXAMPLES

### Example: Determine whether the document tracking site is enabled
```
PS C:\>Get-AadrmDocumentTrackingFeature
```

This command determines whether the Azure Information Protection document tracking feature is enabled.

## PARAMETERS

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Disable-AadrmDocumentTrackingFeature](xref:AADRM/vlatest/Disable-AadrmDocumentTrackingFeature.md)

[Enable-AadrmDocumentTrackingFeature](xref:AADRM/vlatest/Enable-AadrmDocumentTrackingFeature.md)
