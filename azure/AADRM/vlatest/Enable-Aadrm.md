---
external help file: Microsoft.RightsManagementServices.Online.Admin.PowerShell.dll-Help.xml
online version: http://go.microsoft.com/fwlink/?LinkId=400602
schema: 2.0.0
ms.assetid: 60B3F42C-4FEF-435B-AE28-771932FA6251
updated_at: 2/4/2017 5:39 PM
ms.date: 2/4/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/master/Azure%20Information%20Protection/AADRM/vlatest/Enable-Aadrm.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/master/Azure%20Information%20Protection/AADRM/vlatest/Enable-Aadrm.md
gitcommit: https://github.com/Azure/azure-docs-powershell-aip/blob/6ffafc7c33a2088f5b1357f508b53e2bb981e987/Azure%20Information%20Protection/AADRM/vlatest/Enable-Aadrm.md
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

# Enable-Aadrm

## SYNOPSIS
Activates Rights Management for your organization.

## SYNTAX

```
Enable-Aadrm [<CommonParameters>]
```

## DESCRIPTION
The **Enable-Aadrm** cmdlet enables your organization to use Azure Rights Management when you have a subscription that includes this service.
This cmdlet offers an alternative method of activating the Azure Rights Management service rather than using the management portals.
You must activate Rights Management before you can begin to use information rights management (IRM) features in Office applications and before you can protect documents and emails by using other applications that use Azure Rights Management.
When you activate Rights Management, you turn on this service for all rights-enabled applications and services, but some applications and services and might need further configuration before they can use Azure Rights Management.

For more information about activating Rights Management and a link to information about the service plans that include Azure Rights Management, see [Activating Azure Rights Management](https://docs.microsoft.com/rights-management/deploy-use/activate-service) (https://docs.microsoft.com/rights-management/deploy-use/activate-service) on the Microsoft documentation site.
For more information about other deployment steps that might be needed, see the [Deployment Roadmap](https://docs.microsoft.com/rights-management/plan-design/deployment-roadmap)  (https://docs.microsoft.com/rights-management/plan-design/deployment-roadmap).

## EXAMPLES

### Example 1: Enable Rights Management
```
PS C:\>Enable-Aadrm
```

This command activates Rights Management for your organization.

## PARAMETERS

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Disable-Aadrm](xref:AADRM/vlatest/Disable-Aadrm.md)

[Get-Aadrm](xref:AADRM/vlatest/Get-Aadrm.md)

[Activating Azure Rights Management](https://docs.microsoft.com/rights-management/deploy-use/activate-service)

[Deployment Roadmap](https://docs.microsoft.com/rights-management/plan-design/deployment-roadmap)
