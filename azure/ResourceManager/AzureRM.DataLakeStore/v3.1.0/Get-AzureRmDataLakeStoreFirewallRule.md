---
external help file: Microsoft.Azure.Commands.DataLakeStore.dll-Help.xml
ms.assetid: 7D27F7B1-BAF8-4A01-8BA7-A75A4CFAE370
online version: 
schema: 2.0.0
updated_at: 11/8/2016 12:38 AM
ms.date: 11/8/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.DataLakeStore/v3.1.0/Get-AzureRmDataLakeStoreFirewallRule.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.DataLakeStore/v3.1.0/Get-AzureRmDataLakeStoreFirewallRule.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04b9ae2d1c44a3ada330f570237886794cede893/azureps-cmdlets-docs/ResourceManager/AzureRM.DataLakeStore/v3.1.0/Get-AzureRmDataLakeStoreFirewallRule.md
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

# Get-AzureRmDataLakeStoreFirewallRule

## SYNOPSIS
Gets the specified firewall rules in the specified Data Lake Store.
If no firewall rule is specified, then lists all firewall rules for the account.

## SYNTAX

```
Get-AzureRmDataLakeStoreFirewallRule [-Account] <String> [[-Name] <String>] [[-ResourceGroupName] <String>]
```

## DESCRIPTION
The Get-AzureRmDataLakeStoreFirewallRule cmdlet gets the specified firewall rules in the specified Data Lake Store.
If no firewall rule is specified, then lists all firewall rules for the account.

## EXAMPLES

### --------------------------  Example 1: Retrieve a specific firewall rule  --------------------------
@{paragraph=PS C:\\\>}

```
PS C:\> Get-AzureRmDataLakeStoreFirewallRule -AccountName "ContosoADL" -Name MyFirewallRule
```

Returns the firewall rule named "MyFirewallRule" from account "ContosoADL"

### --------------------------  Example 2: List all firewall rules in an account  --------------------------
@{paragraph=PS C:\\\>}

```
PS C:\> Get-AzureRmDataLakeStoreFirewallRule -AccountName "ContosoADL"
```

Returns all firewall rules in account "ContosoADL"

## PARAMETERS

### -Account
The Data Lake Store account to retrieve the firewall rule from.

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
The name of the firewall rule to retrieve

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

### -ResourceGroupName
Name of resource group under which want to retrieve the specified account's specified firewall rule.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

### Microsoft.Azure.Management.DataLake.Store.Models.FirewallRule

### System.Collections.Generic.IList`1[[Microsoft.Azure.Management.DataLake.Store.Models.FirewallRule, Microsoft.Azure.Management.DataLake.Store, Version=0.12.0.0, Culture=neutral, PublicKeyToken=31bf3856ad364e35]]

## NOTES

## RELATED LINKS

