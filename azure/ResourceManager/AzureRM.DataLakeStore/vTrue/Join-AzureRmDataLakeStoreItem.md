---
external help file: Microsoft.Azure.Commands.DataLakeStore.dll-Help.xml
ms.assetid: 4E9EA2E9-4BE2-4530-BC2B-D369C016CD8C
online version: 
schema: 2.0.0
updated_at: 3/4/2017 12:37 AM
ms.date: 3/4/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.DataLakeStore/vTrue/Join-AzureRmDataLakeStoreItem.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.DataLakeStore/vTrue/Join-AzureRmDataLakeStoreItem.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/91cff23a000b99dc60ec82204d789c7ace1d7134/azureps-cmdlets-docs/ResourceManager/AzureRM.DataLakeStore/vTrue/Join-AzureRmDataLakeStoreItem.md
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

# Join-AzureRmDataLakeStoreItem

## SYNOPSIS
Joins one or more files to create one file in Data Lake Store.

## SYNTAX

```
Join-AzureRmDataLakeStoreItem [-Account] <String> [-Paths] <DataLakeStorePathInstance[]>
 [-Destination] <DataLakeStorePathInstance> [-Force] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The **Join-AzureRmDataLakeStoreItem** cmdlet joins one or more files to create one file in Data Lake Store.

## EXAMPLES

### Example 1: Join two items
```
PS C:\>Join-AzureRmDataLakeStoreItem -AccountName "ContosoADL" -Paths "/MyFiles/File01.txt","/MyFiles/File02.txt" -Destination "/MyFiles/CombinedFile.txt"
```

This command joins File01.txt and File02.txt to create the file CombinedFile.txt.

## PARAMETERS

### -Account
Specifies the name of the Data Lake Store account.

```yaml
Type: String
Parameter Sets: (All)
Aliases: AccountName

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Destination
Specifies the Data Lake Store path for the joined item, starting with the root directory (/).

```yaml
Type: DataLakeStorePathInstance
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Force
Indicates that this operation can overwrite the destination file if it already exists.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: 3
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Paths
Specifies an array of Data Lake Store paths of the files to combine, starting with the root directory (/).

```yaml
Type: DataLakeStorePathInstance[]
Parameter Sets: (All)
Aliases: Path

Required: True
Position: 1
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

### string
The full path to the resulting file from the joined files.

## NOTES

## RELATED LINKS

[Get-AzureRmDataLakeStoreItem](xref:ResourceManager/AzureRM.DataLakeStore/vTrue/Get-AzureRmDataLakeStoreItem.md)

[Export-AzureRmDataLakeStoreItem](xref:ResourceManager/AzureRM.DataLakeStore/vTrue/Export-AzureRmDataLakeStoreItem.md)

[Import-AzureRmDataLakeStoreItem](xref:ResourceManager/AzureRM.DataLakeStore/vTrue/Import-AzureRmDataLakeStoreItem.md)

[New-AzureRmDataLakeStoreItem](xref:ResourceManager/AzureRM.DataLakeStore/vTrue/New-AzureRmDataLakeStoreItem.md)

[Remove-AzureRmDataLakeStoreItem](xref:ResourceManager/AzureRM.DataLakeStore/vTrue/Remove-AzureRmDataLakeStoreItem.md)

[Test-AzureRmDataLakeStoreItem](xref:ResourceManager/AzureRM.DataLakeStore/vTrue/Test-AzureRmDataLakeStoreItem.md)


