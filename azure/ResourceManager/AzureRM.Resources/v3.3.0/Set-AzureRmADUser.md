---
external help file: Microsoft.Azure.Commands.Resources.dll-Help.xml
ms.assetid: 388D4173-A937-42FA-81CB-C4A27F9D0B04
online version: 
schema: 2.0.0
updated_at: 3/4/2017 8:24 PM
ms.date: 3/4/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v3.3.0/Set-AzureRmADUser.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v3.3.0/Set-AzureRmADUser.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/8d5bd179154dcb8950eb74b5a9a717acab065233/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v3.3.0/Set-AzureRmADUser.md
ms.topic: reference
ms.prod: powershell
ms.technology: Azure PowerShell
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: False
ms.service: azure-powershell
---

# Set-AzureRmADUser

## SYNOPSIS
Updates an existing active directory user.

## SYNTAX

```
Set-AzureRmADUser -UPNOrObjectId <String> [-DisplayName <String>] [-EnableAccount <Boolean>]
 [-Password <String>] [-ForceChangePasswordNextLogin] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [-WhatIf] [-Confirm]
```

## DESCRIPTION
The **Set-AzureRmADUser** cmdlet updates an existing active directory user.
For more information, see [Update a user](https://msdn.microsoft.com/en-us/library/azure/ad/graph/api/users-operations#UpdateUser) https://msdn.microsoft.com/en-us/library/azure/ad/graph/api/users-operations#UpdateUser.

## EXAMPLES

## PARAMETERS

### -UPNOrObjectId
Specifies the user principal name or the object ID of the user for which this cmdlet updates the properties for.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -DisplayName
Specifies the new name to display in the address book for the user.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -EnableAccount
Indicates whether the cmdlet enables the account.

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Password
Specifies the new password for the user.
It must meet the tenant's password complexity requirements.
It is recommended to set a strong password.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ForceChangePasswordNextLogin
Indicates that the cmdlet forces the user to change the password on next login.
Otherwise it will be ignored.
It must be specified if the user must change the password on the next successful login.
Default behavior is to not change the password on the next successful login.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -InformationAction
Specifies how this cmdlet responds to an information event.

The acceptable values for this parameter are:

- Continue
- Ignore
- Inquire
- SilentlyContinue
- Stop
- Suspend

```yaml
Type: ActionPreference
Parameter Sets: (All)
Aliases: infa

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationVariable
Specifies an information variable.

```yaml
Type: String
Parameter Sets: (All)
Aliases: iv

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureRmADUser](xref:ResourceManager/AzureRM.Resources/v3.3.0/Get-AzureRmADUser.md)

[New-AzureRmADUser](xref:ResourceManager/AzureRM.Resources/v3.3.0/New-AzureRmADUser.md)

[Remove-AzureRmADUser](xref:ResourceManager/AzureRM.Resources/v3.3.0/Remove-AzureRmADUser.md)
