---
external help file: RMSProtection.dll-Help.xml
online version: http://go.microsoft.com/fwlink/?LinkId=734985
schema: 2.0.0
ms.assetid: ED6B146C-069C-4DB2-9477-65D9783BC002
updated_at: 2/4/2017 5:39 PM
ms.date: 2/4/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/master/Azure%20Information%20Protection/RMSProtection/vlatest/Clear-RMSAuthentication.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/master/Azure%20Information%20Protection/RMSProtection/vlatest/Clear-RMSAuthentication.md
gitcommit: https://github.com/Azure/azure-docs-powershell-aip/blob/6ffafc7c33a2088f5b1357f508b53e2bb981e987/Azure%20Information%20Protection/RMSProtection/vlatest/Clear-RMSAuthentication.md
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

# Clear-RMSAuthentication

## SYNOPSIS
Clears credentials for a user who is authenticated to the Azure RMS service.

## SYNTAX

```
Clear-RMSAuthentication [<CommonParameters>]
```

## DESCRIPTION
The **Clear-RMSAuthentication** cmdlet clears the credentials that are used when a user has previously entered their user name and password to authenticate to Azure Rights Management (Azure RMS).

When you enter a user name and password to sign in to Azure RMS, the credentials are cached on the computer. Because these cached credentials are used across PowerShell sessions, to sign in as a different user, you must first run **Clear-RMSAuthentication**. You are then prompted for new credentials.

This cmdlet applies to Azure RMS only and when you authenticate as a user rather than a service principal. It does not apply to AD RMS.

Note: If you want to clear the credentials for a service principal that you specified with [Set-RMSServerAuthentication](./Set-RMSServerAuthentication), close your PowerShell session and start a new session that runs **Set-RMSServerAuthentication** with the new credentials.

## EXAMPLES

### Example 1: Clear authentication credentials
```
PS C:\>Clear-RMSAuthentication                        
Authentication cleared
```

This command clears the currently cached authentication credentials for a user who is authenticated to Azure RMS on a computer that is not joined to a domain.

## PARAMETERS

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Set-RMSServerAuthentication](xref:RMSProtection/vlatest/Set-RMSServerAuthentication.md)
