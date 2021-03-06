---
external help file: Microsoft.WindowsAzure.Commands.Storage.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 32856CD6-74E8-4527-8CC7-175FA6AC8085
updated_at: 11/11/2016 11:03 PM
ms.date: 11/11/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/Storage/Azure.Storage/v2.2.0/Get-AzureStorageQueue.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/Storage/Azure.Storage/v2.2.0/Get-AzureStorageQueue.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/79eeb985ea480979357fb4695832a0c3d29a48bf/azureps-cmdlets-docs/Storage/Azure.Storage/v2.2.0/Get-AzureStorageQueue.md
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

# Get-AzureStorageQueue

## SYNOPSIS
Lists storage queues.

## SYNTAX

### QueueName (Default)
```
Get-AzureStorageQueue [[-Name] <String>] [-Context <AzureStorageContext>] [-PipelineVariable <String>]
 [<CommonParameters>]
```

### QueuePrefix
```
Get-AzureStorageQueue -Prefix <String> [-Context <AzureStorageContext>] [-PipelineVariable <String>]
 [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureStorageQueue** cmdlet lists storage queues associated with an Azure Storage account.

## EXAMPLES

### Example 1: List all Azure Storage queues
```
PS C:\>Get-AzureStorageQueue
```

This command gets a list of all storage queues for the current Storage account.

### Example 2: List Azure Storage queues using a wildcard character
```
PS C:\>Get-AzureStorageQueue -Name queue*
```

This command uses a wildcard character to get a list of storage queues whose name starts with queue.

### Example 3: List Azure Storage queues using queue name prefix
```
PS C:\>Get-AzureStorageQueue -Prefix "queue"
```

This example uses the *Prefix* parameter to get a list of storage queues whose name starts with queue.

## PARAMETERS

### -Name
Specifies a name.
If no name is specified, the cmdlet gets a list of all the queues.
If a full or partial name is specified, the cmdlet gets all queues that match the name pattern.

```yaml
Type: String
Parameter Sets: QueueName
Aliases: N, Queue

Required: False
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -Context
Specifies the Azure storage context.
You can create it by using the **New-AzureStorageContext** cmdlet.

```yaml
Type: AzureStorageContext
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -Prefix
Specifies a prefix used in the name of the queues you want to get.

```yaml
Type: String
Parameter Sets: QueuePrefix
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PipelineVariable
Stores the value of the current pipeline element as a variable, for any named command as it flows through the pipeline.

```yaml
Type: String
Parameter Sets: (All)
Aliases: pv

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

## NOTES

## RELATED LINKS

[New-AzureStorageQueue](xref:Storage/Azure.Storage/v2.2.0/New-AzureStorageQueue.md)

[Remove-AzureStorageQueue](xref:Storage/Azure.Storage/v2.2.0/Remove-AzureStorageQueue.md)


