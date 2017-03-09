---
external help file: Microsoft.Azure.Commands.ServiceBus.dll-Help.xml
online version: 
schema: 2.0.0
updated_at: 3/9/2017 2:12 AM
ms.date: 3/9/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.ServiceBus/vTrue/Remove-AzureRmServiceBusQueue.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.ServiceBus/vTrue/Remove-AzureRmServiceBusQueue.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/fd4b3c7c85da22d54497dd2e4e5acda28e29fba3/azureps-cmdlets-docs/ResourceManager/AzureRM.ServiceBus/vTrue/Remove-AzureRmServiceBusQueue.md
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

# Remove-AzureRmServiceBusQueue

## SYNOPSIS
Removes the queue from the specified Service Bus namespace.

## SYNTAX

```
Remove-AzureRmServiceBusQueue [-ResourceGroup] <String> [-NamespaceName] <String> [-QueueName] <String>
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureRmServiceBusQueue** cmdlet removes the queue from the specified Service Bus namespace.

## EXAMPLES

### Example 1: Remove the specified queue from a namespace
```
PS C:\> Remove-AzureRmServiceBusQueue -ResourceGroup "Default-ServiceBus-WestUS" -NamespaceName "SB-Example1" -QueueName "SB-Queue_example1"
```

This command removes the queue named SB-Queue_example1 from the namespace named SB-Example1.

## PARAMETERS

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -NamespaceName
Specifies the name of the Service Bus namespace.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -QueueName
Specifies the name of the Service Bus queue.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
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

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
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
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### -ResourceGroup
 System.String

### -NamespaceName
 System.String

### -QueueName
 System.String

## OUTPUTS

### System.Object

## NOTES

## RELATED LINKS

[Get-AzureRmServiceBusTopic](xref:ResourceManager/AzureRM.ServiceBus/vTrue/Get-AzureRmServiceBusTopic.md)

[New-AzureRmServiceBusTopic](xref:ResourceManager/AzureRM.ServiceBus/vTrue/New-AzureRmServiceBusTopic.md)

[Set-AzureRmServiceBusTopic](xref:ResourceManager/AzureRM.ServiceBus/vTrue/Set-AzureRmServiceBusTopic.md)
