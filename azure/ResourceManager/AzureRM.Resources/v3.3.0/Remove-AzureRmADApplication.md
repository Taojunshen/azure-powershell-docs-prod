---
external help file: Microsoft.Azure.Commands.Resources.dll-Help.xml
ms.assetid: C791C593-F7D5-4961-97F9-E4909813FFE7
online version: 
schema: 2.0.0
updated_at: 3/4/2017 6:58 PM
ms.date: 3/4/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v3.3.0/Remove-AzureRmADApplication.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v3.3.0/Remove-AzureRmADApplication.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/aa2ae758d5790a27662a17dfad5119b5b8987494/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v3.3.0/Remove-AzureRmADApplication.md
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

# Remove-AzureRmADApplication

## SYNOPSIS
Removes the Azure Active Directory application.

## SYNTAX

```
Remove-AzureRmADApplication -ObjectId <Guid> [-Force] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [-WhatIf] [-Confirm]
```

## DESCRIPTION
The **Remove-AzureRmADApplication** cmdlet removes the Azure Active Directory application.

## EXAMPLES

### Example 1: Delete and Azure Active Directory application


```
PS C:\> Remove-AzureRmADApplication -ObjectId b4cd1619-80b3-4cfb-9f8f-9f2333425738 -Force
```

This command removes the specified Azure Active Directory application.

## PARAMETERS

### -ObjectId
Specifies the object ID of the application that this cmdlet removes.

```yaml
Type: Guid
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Force
Forces the command to run without asking for user confirmation.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
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
Keywords: azure, azurerm, arm, resource, management, manager, resource, group, template, deployment

## RELATED LINKS

[New-AzureRmADApplication](xref:ResourceManager/AzureRM.Resources/v3.3.0/New-AzureRmADApplication.md)

[Get-AzureRmADApplication](xref:ResourceManager/AzureRM.Resources/v3.3.0/Get-AzureRmADApplication.md)

[Set-AzureRmADApplication](xref:ResourceManager/AzureRM.Resources/v3.3.0/Set-AzureRmADApplication.md)

[Remove-AzureRmADAppCredential](xref:ResourceManager/AzureRM.Resources/v3.3.0/Remove-AzureRmADAppCredential.md)
