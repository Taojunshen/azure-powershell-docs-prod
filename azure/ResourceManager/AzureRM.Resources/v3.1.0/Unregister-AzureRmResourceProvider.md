---
external help file: Microsoft.Azure.Commands.ResourceManager.Cmdlets.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: B373AC40-6BED-44A7-80B7-AB3A8FE9B8A3
updated_at: 1/9/2017 11:25 PM
ms.date: 1/9/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v3.1.0/Unregister-AzureRmResourceProvider.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v3.1.0/Unregister-AzureRmResourceProvider.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/909020b7dbd03ec23a61b4fe16ccd2762277084c/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v3.1.0/Unregister-AzureRmResourceProvider.md
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

# Unregister-AzureRmResourceProvider

## SYNOPSIS
Unregisters a resource provider.

## SYNTAX

```
Unregister-AzureRmResourceProvider -ProviderNamespace <String> [-ApiVersion <String>] [-Pre] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The **Unregister-AzureRmResourceProvider** cmdlet unregisters an Azure resource provider.

## EXAMPLES


## PARAMETERS

### -ProviderNamespace
Specifies the namespace of the resource provider.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ApiVersion
Specifies the API version that is supported by the resource Provider.
You can specify a different version than the default version.

```yaml
Type: String
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

### -Pre
Indicates that this cmdlet considers pre-release API versions when it automatically determines which version to use.

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

## NOTES

## RELATED LINKS

[Get-AzureRmResourceProvider](xref:ResourceManager/AzureRM.Resources/v3.1.0/Get-AzureRmResourceProvider.md)

[Register-AzureRmResourceProvider](xref:ResourceManager/AzureRM.Resources/v3.1.0/Register-AzureRmResourceProvider.md)


