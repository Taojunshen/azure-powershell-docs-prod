---
external help file: Microsoft.Azure.Commands.DataLakeStore.dll-Help.xml
ms.assetid: 6C7A7E1A-87A2-4F0D-9091-413C111F47F0
online version: 
schema: 2.0.0
updated_at: 3/4/2017 9:58 PM
ms.date: 3/4/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ResourceManager/AzureRM.DataLakeStore/v3.3.0/Remove-AzureRmDataLakeStoreFirewallRule.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ResourceManager/AzureRM.DataLakeStore/v3.3.0/Remove-AzureRmDataLakeStoreFirewallRule.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/7761f732d57261bdc233763ac2d243d320e93043/azureps-cmdlets-docs/ResourceManager/AzureRM.DataLakeStore/v3.3.0/Remove-AzureRmDataLakeStoreFirewallRule.md
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

# Remove-AzureRmDataLakeStoreFirewallRule

## SYNOPSIS
Removes the specified firewall rule in the specified Data Lake Store.

## SYNTAX

```
Remove-AzureRmDataLakeStoreFirewallRule [-Account] <String> [[-Name] <String>] [-PassThru]
 [[-ResourceGroupName] <String>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureRmDataLakeStoreFirewallRule** cmdlet removes the specified firewall rule in the specified Data Lake Store.

## EXAMPLES

###  Example 1: Remove a firewall rule from an account
```
PS C:\> Remove-AzureRmDataLakeStoreFirewallRule -AccountName "ContosoADL" -Name MyFirewallRule
```

This command removes the firewall rule named MyFirewallRule from the account named ContosoADL.

## PARAMETERS

### -Account
Specifies the Data Lake Store account that this cmdlet updates the firewall rule.

```yaml
Type: String
Parameter Sets: (All)
Aliases: AccountName

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Name
Specifies the name of the firewall rule that this cmdlet removes.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -PassThru
Returns an object representing the item with which you are working. By default, this cmdlet does not generate any output.

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

### -ResourceGroupName
Specifies the name of the resource group that contains the account that this cmdlet removes the firewall rule.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 4
Default value: None
Accept pipeline input: True (ByPropertyName)
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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### System.Boolean

## NOTES

## RELATED LINKS

[Add-AzureRmDataLakeStoreFirewallRule](xref:ResourceManager/AzureRM.DataLakeStore/v3.3.0/Add-AzureRmDataLakeStoreFirewallRule.md)

[Get-AzureRmDataLakeStoreFirewallRule](xref:ResourceManager/AzureRM.DataLakeStore/v3.3.0/Get-AzureRmDataLakeStoreFirewallRule.md)

[Set-AzureRmDataLakeStoreFirewallRule](xref:ResourceManager/AzureRM.DataLakeStore/v3.3.0/Set-AzureRmDataLakeStoreFirewallRule.md)
