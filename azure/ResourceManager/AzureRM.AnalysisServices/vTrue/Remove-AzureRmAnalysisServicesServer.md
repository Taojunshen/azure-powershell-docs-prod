---
external help file: Microsoft.Azure.Commands.AnalysisServices.dll-Help.xml
online version: 
schema: 2.0.0
updated_at: 3/4/2017 12:37 AM
ms.date: 3/4/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ResourceManager/AzureRM.AnalysisServices/vTrue/Remove-AzureRmAnalysisServicesServer.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ResourceManager/AzureRM.AnalysisServices/vTrue/Remove-AzureRmAnalysisServicesServer.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/91cff23a000b99dc60ec82204d789c7ace1d7134/azureps-cmdlets-docs/ResourceManager/AzureRM.AnalysisServices/vTrue/Remove-AzureRmAnalysisServicesServer.md
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

# Remove-AzureRmAnalysisServicesServer

## SYNOPSIS
Deletes an instance of Analysis Services server

## SYNTAX

```
Remove-AzureRmAnalysisServicesServer [-Name] <String> [[-ResourceGroupName] <String>] [-PassThru] [-WhatIf]
 [-Confirm]
```

## DESCRIPTION
The Remove-AzureRmAnalysisServicesServer cmdlet  deletes an instance of Analysis Services server

## EXAMPLES

### Example 1
```
PS C:\> Remove-AzureRmAnalysisServicesServer -Name "testserver" -ResourceGroupName "testgroup"
```

This command will remove the server named testserver in the resourcegroup testgroup

## PARAMETERS

### -Name
Name of the Analysis Services server

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

### -PassThru
Will return the deleted server details if the operation completes successfully

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

### -ResourceGroupName
Name of the Azure resource group to which the server belongs

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

### -Confirm
Prompts user to confirm whether to perform the operation

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
Describes the actions the current operation will perform without actually performing them

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

## INPUTS

## OUTPUTS

### Microsoft.Azure.Commands.AnalysisServices.Models.AzureAnalysisServicesServer

## NOTES
Alias: Remove-AzureAs

## RELATED LINKS

[Get-AzureRmAnalysisServicesServer](xref:ResourceManager/AzureRM.AnalysisServices/vTrue/Get-AzureRmAnalysisServicesServer.md)

[New-AzureRmAnalysisServicesServer](xref:ResourceManager/AzureRM.AnalysisServices/vTrue/New-AzureRmAnalysisServicesServer.md)
