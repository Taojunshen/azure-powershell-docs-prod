---
external help file: Microsoft.Azure.Commands.ServiceBus.dll-Help.xml
online version: 
schema: 2.0.0
updated_at: 3/9/2017 2:12 AM
ms.date: 3/9/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.ServiceBus/vTrue/Remove-AzureRmServiceBusNamespaceAuthorizationRule.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.ServiceBus/vTrue/Remove-AzureRmServiceBusNamespaceAuthorizationRule.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/fd4b3c7c85da22d54497dd2e4e5acda28e29fba3/azureps-cmdlets-docs/ResourceManager/AzureRM.ServiceBus/vTrue/Remove-AzureRmServiceBusNamespaceAuthorizationRule.md
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

# Remove-AzureRmServiceBusNamespaceAuthorizationRule

## SYNOPSIS
Removes the authorization rule of a Service Bus namespace from the specified resource group.

## SYNTAX

```
Remove-AzureRmServiceBusNamespaceAuthorizationRule [-ResourceGroup] <String> [-NamespaceName] <String>
 [-AuthorizationRuleName] <String> [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureRmServiceBusNamespaceAuthorizationRule** cmdlet removes the authorization rule of a Service Bus namespace for the specified resource group.

## EXAMPLES

### Example 1: Remove an authorization rule of a Service Bus namespace from a resource group
```
PS C:\> Remove-AzureRmServiceBusNamespaceAuthorizationRule -ResourceGroup "Default-ServiceBus-WestUS" -NamespaceName "SB-Example1" -AuthorizationRuleName "AuthoRule1"
```

This command removes the authorization rule named SBAuthoRule1 of the namespace named SB-Example1 from the resource group named SB-Example1.

## PARAMETERS

### -AuthorizationRuleName
Specifies the name of the namespace authorization rule.

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

### -AuthorizationRuleName
 System.String

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureRmServiceBusNamespaceAuthorizationRule](xref:ResourceManager/AzureRM.ServiceBus/vTrue/Get-AzureRmServiceBusNamespaceAuthorizationRule.md)

[New-AzureRmServiceBusNamespaceAuthorizationRule](xref:ResourceManager/AzureRM.ServiceBus/vTrue/New-AzureRmServiceBusNamespaceAuthorizationRule.md)

[Set-AzureRmServiceBusNamespaceAuthorizationRule](xref:ResourceManager/AzureRM.ServiceBus/vTrue/Set-AzureRmServiceBusNamespaceAuthorizationRule.md)
