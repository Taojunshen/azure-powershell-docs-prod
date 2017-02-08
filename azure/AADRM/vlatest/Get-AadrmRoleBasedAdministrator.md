---
external help file: Microsoft.RightsManagementServices.Online.Admin.PowerShell.dll-Help.xml
online version: http://go.microsoft.com/fwlink/?LinkId=400613
schema: 2.0.0
ms.assetid: 528FCC5D-F653-4B40-8D82-F036BAB66E5C
updated_at: 2/8/2017 6:01 PM
ms.date: 2/8/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/master/Azure%20Information%20Protection/AADRM/vlatest/Get-AadrmRoleBasedAdministrator.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/master/Azure%20Information%20Protection/AADRM/vlatest/Get-AadrmRoleBasedAdministrator.md
gitcommit: https://github.com/Azure/azure-docs-powershell-aip/blob/b5b814c02caa6cd576a3db614749957f10782144/Azure%20Information%20Protection/AADRM/vlatest/Get-AadrmRoleBasedAdministrator.md
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

# Get-AadrmRoleBasedAdministrator

## SYNOPSIS
Gets the role-based administrators for Rights Management.

## SYNTAX

```
Get-AadrmRoleBasedAdministrator [-Role <Role>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AadrmRoleBasedAdministrator** cmdlet gets the role-based administrators for Azure Rights Management. You can get the administrators for a specified role.

## EXAMPLES

### Example 1: List administrators
```
PS C:\>Get-AadrmRoleBasedAdministrator
```

This command lists the role-based administrators for Rights Management.

## PARAMETERS

### -Role
Specifies a role. The cmdlet gets the administrators that belong to the role that you specify.

The acceptable values for this parameter are:

- ConnectorAdministrator
- GlobalAdministrator

```yaml
Type: Role
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Add-AadrmRoleBasedAdministrator](xref:AADRM/vlatest/Add-AadrmRoleBasedAdministrator.md)

[Remove-AadrmRoleBasedAdministrator](xref:AADRM/vlatest/Remove-AadrmRoleBasedAdministrator.md)
