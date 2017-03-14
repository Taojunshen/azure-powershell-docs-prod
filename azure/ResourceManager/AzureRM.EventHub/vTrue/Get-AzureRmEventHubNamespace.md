---
external help file: Microsoft.Azure.Commands.EventHub.dll-Help.xml
online version: 
schema: 2.0.0
updated_at: 3/10/2017 7:40 PM
ms.date: 3/10/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ResourceManager/AzureRM.EventHub/vTrue/Get-AzureRmEventHubNamespace.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ResourceManager/AzureRM.EventHub/vTrue/Get-AzureRmEventHubNamespace.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/16665bd43882b185a8143de54e498a0463907aa7/azureps-cmdlets-docs/ResourceManager/AzureRM.EventHub/vTrue/Get-AzureRmEventHubNamespace.md
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

# Get-AzureRmEventHubNamespace

## SYNOPSIS
Gets the details of an Event Hubs namespace, or gets a list of all Event Hubs namespaces in the current Azure subscription.

## SYNTAX

```
Get-AzureRmEventHubNamespace [[-ResourceGroupName] <String>] [[-NamespaceName] <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmEventHubNamespace** cmdlet gets either the details of a specified Event Hubs namespace, or a list of all Event Hubs namespaces in the current Azure subscription. If the namespace name is provided, the details of a single Event Hubs namespace is returned. If the namespace name is not provided, a list of namespaces is returned.

## EXAMPLES

### Example 1
```
PS C:\> Get-AzureRmEventHubNamespace -ResourceGroupName MyResourceGroupName -NamespaceName MyNamespaceName
```

Gets the details of the Event Hubs namespace `MyNamespaceName` in the resource group `MyResourceGroupName`.

## PARAMETERS

### -NamespaceName
The Event Hubs namespace name.

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
Resource group name.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.String

## OUTPUTS

### System.Collections.Generic.List`1[[Microsoft.Azure.Commands.EventHub.Models.NamespaceAttributes, Microsoft.Azure.Commands.EventHub, Version=0.0.1.0, Culture=neutral, PublicKeyToken=null]]

## NOTES

## RELATED LINKS

