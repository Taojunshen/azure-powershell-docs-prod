---
external help file: Microsoft.Azure.Commands.Compute.dll-Help.xml
ms.assetid: 6442E5BB-D59D-483B-8AC5-2586C6C1E925
online version: 
schema: 2.0.0
updated_at: 3/4/2017 12:37 AM
ms.date: 3/4/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ResourceManager/AzureRM.Compute/vTrue/Set-AzureRmVmss.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ResourceManager/AzureRM.Compute/vTrue/Set-AzureRmVmss.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/91cff23a000b99dc60ec82204d789c7ace1d7134/azureps-cmdlets-docs/ResourceManager/AzureRM.Compute/vTrue/Set-AzureRmVmss.md
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

# Set-AzureRmVmss

## SYNOPSIS
Sets specific actions on a specified VMSS.

## SYNTAX

### InvokeByDynamicParameters (Default)
```
Set-AzureRmVmss [-WhatIf] [-Confirm] [-ResourceGroupName] <String> [-VMScaleSetName] <String> [-Reimage]
 [<CommonParameters>]
```

### InvokeByDynamicParametersForFriendMethod
```
Set-AzureRmVmss [-WhatIf] [-Confirm] [-ResourceGroupName] <String> [-VMScaleSetName] <String> [-ReimageAll]
 [<CommonParameters>]
```

## DESCRIPTION
The **Set-AzureRmVmss** cmdlet sets specific actions on the Virtual Machine Scale Set (VMSS).
The only action this cmdlet supports is Reimage.

## EXAMPLES

### Example 1: Reimage a VMSS
```
PS C:\>Set-AzureRmVmss -Reimage -ResourceGroupName "ContosoGroup" -VMScaleSetName "ContosoVMSS"
```

This command reimages the VMSS named ContosoVMSS that belongs to the resource group named ContosoGroup.

## PARAMETERS

### -Reimage
Indicates that the cmdlet reimages the VMSS.

```yaml
Type: SwitchParameter
Parameter Sets: InvokeByDynamicParameters
Aliases: 

Required: True
Position: 4
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ReimageAll
Indicates that the cmdlet reimages all the disks in the VMSS.

```yaml
Type: SwitchParameter
Parameter Sets: InvokeByDynamicParametersForFriendMethod
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of the resource group of the VMSS.

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

### -VMScaleSetName
Species the name of the VMSS for which this cmdlet sets actions on.

```yaml
Type: String
Parameter Sets: (All)
Aliases: Name

Required: True
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
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs. The cmdlet is not run.

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

### This cmdlet does not generate any output.

## NOTES

## RELATED LINKS

[Get-AzureRmVmss](xref:ResourceManager/AzureRM.Compute/vTrue/Get-AzureRmVmss.md)

[New-AzureRmVmss](xref:ResourceManager/AzureRM.Compute/vTrue/New-AzureRmVmss.md)

[Remove-AzureRmVmss](xref:ResourceManager/AzureRM.Compute/vTrue/Remove-AzureRmVmss.md)

[Restart-AzureRmVmss](xref:ResourceManager/AzureRM.Compute/vTrue/Restart-AzureRmVmss.md)

[Start-AzureRmVmss](xref:ResourceManager/AzureRM.Compute/vTrue/Start-AzureRmVmss.md)

[Stop-AzureRmVmss](xref:ResourceManager/AzureRM.Compute/vTrue/Stop-AzureRmVmss.md)

[Update-AzureRmVmss](xref:ResourceManager/AzureRM.Compute/vTrue/Update-AzureRmVmss.md)


