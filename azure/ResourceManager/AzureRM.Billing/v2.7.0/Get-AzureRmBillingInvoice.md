---
external help file: Microsoft.Azure.Commands.Billing.dll-Help.xml
online version: 
schema: 2.0.0
updated_at: 3/11/2017 2:20 AM
ms.date: 3/11/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Billing/v2.7.0/Get-AzureRmBillingInvoice.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Billing/v2.7.0/Get-AzureRmBillingInvoice.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04f63f6e685743ace2c57eb157574e34e8610b1c/azureps-cmdlets-docs/ResourceManager/AzureRM.Billing/v2.7.0/Get-AzureRmBillingInvoice.md
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

# Get-AzureRmBillingInvoice

## SYNOPSIS
Get billing invoices of the subscription.

## SYNTAX

### List (Default)
```
Get-AzureRmBillingInvoice [-MaxCount <Int32>] [-GenerateDownloadUrl] [<CommonParameters>]
```

### Latest
```
Get-AzureRmBillingInvoice [-Latest] [<CommonParameters>]
```

### Single
```
Get-AzureRmBillingInvoice -Name <String> [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmBillingInvoice** cmdlet gets billing invoices of the subscription. 

## EXAMPLES

### Example 1
```
PS C:\> Get-AzureRmBillingInvoice -Latest
```

Get the latest invoice of the subscription.

### Example 2
```
PS C:\> Get-AzureRmBillingInvoice -Name 2017-02-18-432543543
```

Get the invoice of the subscription with the specified name.

### Example 3
```
PS C:\> Get-AzureRmBillingInvoice
```

Get all available invoices of the subscription in reverse chronological order beginning with the most recent invoice without download Url. 

### Example 4
```
PS C:\> Get-AzureRmBillingInvoice -GenerateDownloadUrl -MaxCount 10
```

Get most recent 10 invoices of the subscription and include the download Url in the result.

## PARAMETERS

### -GenerateDownloadUrl
Generate the download url of the invoices.```yaml
Type: SwitchParameter
Parameter Sets: List
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Latest
Get the latest invoice.```yaml
Type: SwitchParameter
Parameter Sets: Latest
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MaxCount
Determines the maximum number of records to return.

```yaml
Type: Int32
Parameter Sets: List
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
Name of a specific invoice to get or the most recent if not specified.```yaml
Type: String
Parameter Sets: Single
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None

## OUTPUTS

### System.Collections.Generic.List`1[[Microsoft.Azure.Management.Billing.Models.Invoice, Microsoft.Azure.Commands.Billing, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null]]
Microsoft.Azure.Management.Billing.Models.Invoice

## NOTES

## RELATED LINKS

