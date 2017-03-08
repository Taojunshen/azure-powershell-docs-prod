---
external help file: Microsoft.Azure.Commands.ServiceBus.dll-Help.xml
online version: 
schema: 2.0.0
updated_at: 3/8/2017 6:26 PM
ms.date: 3/8/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ResourceManager/AzureRM.ServiceBus/vTrue/Get-AzureRmServiceBusNamespace.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ResourceManager/AzureRM.ServiceBus/vTrue/Get-AzureRmServiceBusNamespace.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/7476628ef2747b1b2e855d4dba9a381d15ff82a6/azureps-cmdlets-docs/ResourceManager/AzureRM.ServiceBus/vTrue/Get-AzureRmServiceBusNamespace.md
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

# Get-AzureRmServiceBusNamespace

## SYNOPSIS
Gets a description for the specified Service Bus namespace within the resource group.

## SYNTAX

```
Get-AzureRmServiceBusNamespace [[-ResourceGroup] <String>] [[-NamespaceName] <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmServiceBusNamespace** cmdlet gets a description for the specified Service Bus namespace within the resource group.

## EXAMPLES

### Example 1: Get a description of the specified Service bus namespace
```
PS C:\> Get-AzureRmServiceBusNamespace -ResourceGroup "Default-ServiceBus-WestUS" -NamespaceName "SB-Example1"
```

This command gets a description of the Service Bus namespace named SB-Example1.

## PARAMETERS

### -NamespaceName
Specifies the name of the Service Bus namespace.

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

### -ResourceGroup
Specifies the name of the resource group.

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

### -ResourceGroup
System.String

### -NamespaceName
 System.String

## OUTPUTS

### System.Collections.Generic.List`1[[Microsoft.Azure.Commands.ServiceBus.Models.NamespaceAttributes, Microsoft.Azure.Commands.ServiceBus, Version=0.0.1.0, Culture=neutral, PublicKeyToken=null]]
Name               : SB-Example1
Id                 : /subscriptions/854d368f-1828-428f-8f3c-f2affa9b2f7d/resourceGroups/Default-ServiceBus-WestUS/providers/Microsoft.ServiceBus/namespaces/SB-Example1
Location           : West US
Sku                : Name : Standard , Capacity : 1 , Tier : Standard
ProvisioningState  : Succeeded
Status             : Active
CreatedAt          : 1/20/2017 1:40:01 AM
UpdatedAt          : 1/20/2017 1:40:24 AM
ServiceBusEndpoint : https://SB-Example1.servicebus.windows.net:443/
Enabled            : True

## NOTES

## RELATED LINKS

[New-AzureRmServiceBusNamespace](xref:ResourceManager/AzureRM.ServiceBus/vTrue/New-AzureRmServiceBusNamespace.md)

[Remove-AzureRmServiceBusNamespace](xref:ResourceManager/AzureRM.ServiceBus/vTrue/Remove-AzureRmServiceBusNamespace.md)

[Set-AzureRmServiceBusNamespace](xref:ResourceManager/AzureRM.ServiceBus/vTrue/Set-AzureRmServiceBusNamespace.md)
