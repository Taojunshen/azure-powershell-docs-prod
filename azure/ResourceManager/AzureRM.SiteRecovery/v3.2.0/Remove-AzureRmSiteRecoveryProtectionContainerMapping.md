---
external help file: Microsoft.Azure.Commands.SiteRecovery.dll-Help.xml
ms.assetid: A04E7EF3-4EBC-46B3-9DE6-66BB94FB0940
online version: 
schema: 2.0.0
updated_at: 11/8/2016 12:38 AM
ms.date: 11/8/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.SiteRecovery/v3.2.0/Remove-AzureRmSiteRecoveryProtectionContainerMapping.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04b9ae2d1c44a3ada330f570237886794cede893/azureps-cmdlets-docs/ResourceManager/AzureRM.SiteRecovery/v3.2.0/Remove-AzureRmSiteRecoveryProtectionContainerMapping.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Remove-AzureRmSiteRecoveryProtectionContainerMapping

## SYNOPSIS
Removes an Azure Site Recovery Protection Container mapping.

## SYNTAX

```
Remove-AzureRmSiteRecoveryProtectionContainerMapping
 -ProtectionContainerMapping <ASRProtectionContainerMapping> [-Force] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureRmSiteRecoveryProtectionContainerMapping** cmdlet removes an Azure Site Recovery Protection Container mapping.

## EXAMPLES

## PARAMETERS

### -ProtectionContainerMapping
Specifies the Azure Site Recovery Protection Container mapping object.

```yaml
Type: ASRProtectionContainerMapping
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Force
Forces the command to run without asking for user confirmation.

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

## OUTPUTS

### Microsoft.Azure.Commands.SiteRecovery.ASRJob

## NOTES

## RELATED LINKS

[Get-AzureRmSiteRecoveryProtectionContainerMapping](xref:ResourceManager/AzureRM.SiteRecovery/v3.2.0/Get-AzureRmSiteRecoveryProtectionContainerMapping.md)

[New-AzureRmSiteRecoveryProtectionContainerMapping](xref:ResourceManager/AzureRM.SiteRecovery/v3.2.0/New-AzureRmSiteRecoveryProtectionContainerMapping.md)