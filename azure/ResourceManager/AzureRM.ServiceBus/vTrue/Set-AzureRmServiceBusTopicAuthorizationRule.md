---
external help file: Microsoft.Azure.Commands.ServiceBus.dll-Help.xml
online version: 
schema: 2.0.0
updated_at: 3/9/2017 6:46 PM
ms.date: 3/9/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ResourceManager/AzureRM.ServiceBus/vTrue/Set-AzureRmServiceBusTopicAuthorizationRule.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ResourceManager/AzureRM.ServiceBus/vTrue/Set-AzureRmServiceBusTopicAuthorizationRule.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/71cac14758de8eeb36a92b82dae146511ac2a136/azureps-cmdlets-docs/ResourceManager/AzureRM.ServiceBus/vTrue/Set-AzureRmServiceBusTopicAuthorizationRule.md
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

# Set-AzureRmServiceBusTopicAuthorizationRule

## SYNOPSIS
Updates the specified authorization rule description for the given Service Bus topic.

## SYNTAX

```
Set-AzureRmServiceBusTopicAuthorizationRule [-ResourceGroup] <String> [-NamespaceName] <String>
 [-TopicName] <String> [-AuthRuleObj] <SharedAccessAuthorizationRuleAttributes>
 [[-AuthorizationRuleName] <String>] [[-Rights] <String[]>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The **Set-AzureRmServiceBusTopicAuthorizationRule** cmdlet updates the description for the specified authorization rule of the given Service Bus topic.

## EXAMPLES

### Example 1: Update the description for an authorization rule
```
PS C:\> $authRuleObj = Get-AzureRmServiceBusTopicAuthorizationRule -ResourceGroup Default-ServiceBus-WestUS -NamespaceName SB-Example1 -TopicName SB-Topic_exampl1 -AuthorizationRuleName SBTopicAuthoRule1

PS C:\> $authRuleObj.Rights.Add("Manage")

PS C:\> Set-AzureRmServiceBusTopicAuthorizationRule -ResourceGroup Default-ServiceBus-WestUS -NamespaceName SB-Example1 -TopicName SB-Topic_exampl1 -AuthRuleObj $authRuleObj
```

This example adds **Manage** to the access rights of the authorization rule named SBTopicAuthoRule1 on the topic named SB-Topic_exampl1.

## PARAMETERS

### -AuthRuleObj
Specifies the Service Bus topic authorization rule object.

```yaml
Type: SharedAccessAuthorizationRuleAttributes
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -AuthorizationRuleName
Specifies the name of the authorization rule. 

This parameter is required if the *AuthruleObj* parameter is not specified.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 3
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

### -Rights
Specifies the rights; for instance, 
@("Listen","Send","Manage"). Required if **-AuthruleObj** is not specified.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: 4
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -TopicName
Specifies the name of the Service Bus topic.

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

### -TopicName
 System.String

### -AuthRuleObj
 Microsoft.Azure.Commands.ServiceBus.Models.SharedAccessAuthorizationRuleAttributes

## OUTPUTS

### Microsoft.Azure.Commands.ServiceBus.Models.SharedAccessAuthorizationRuleAttributes
Id       : /subscriptions/854d368f-1828-428f-8f3c-f2affa9b2f7d/resourceGroups/Default-ServiceBus-WestUS/providers/Microsoft.ServiceBus/namespaces/SB-Example1/topics/SB-Topic_exampl1/authorization
           Rules/SBTopicAuthoRule1
Type     : Microsoft.ServiceBus/AuthorizationRules
Name     : SBTopicAuthoRule1
Location : West US
Tags     : 
Rights   : {Listen, Send, Manage}

## NOTES

## RELATED LINKS

[Get-AzureRmServiceBusTopicAuthorizationRule](xref:ResourceManager/AzureRM.ServiceBus/vTrue/Get-AzureRmServiceBusTopicAuthorizationRule.md)

[New-AzureRmServiceBusTopicAuthorizationRule](xref:ResourceManager/AzureRM.ServiceBus/vTrue/New-AzureRmServiceBusTopicAuthorizationRule.md)

[Remove-AzureRmServiceBusTopicAuthorizationRule](xref:ResourceManager/AzureRM.ServiceBus/vTrue/Remove-AzureRmServiceBusTopicAuthorizationRule.md)
