---
external help file: Microsoft.Azure.Commands.DataLakeStore.dll-Help.xml
ms.assetid: ECA70C6C-E0B0-445D-BCAD-041625FAC632
online version: 
schema: 2.0.0
updated_at: 3/14/2017 9:28 PM
ms.date: 3/14/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ResourceManager/AzureRM.DataLakeStore/v3.4.0/Get-AzureRmDataLakeStoreItem.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ResourceManager/AzureRM.DataLakeStore/v3.4.0/Get-AzureRmDataLakeStoreItem.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/d8384dc6d4871e100f6fbe8e7ea2f22a27c908c2/azureps-cmdlets-docs/ResourceManager/AzureRM.DataLakeStore/v3.4.0/Get-AzureRmDataLakeStoreItem.md
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

# Get-AzureRmDataLakeStoreItem

## SYNOPSIS
Gets the details of a file or folder in Data Lake Store.

## SYNTAX

```
Get-AzureRmDataLakeStoreItem [-Account] <String> [-Path] <DataLakeStorePathInstance> [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmDataLakeStoreItem** cmdlet gets the details of a file or folder in Data Lake Store.

## EXAMPLES

### Example 1: Get details of a file from the Data Lake Store
```
PS C:\> Get-AzureRmDataLakeStoreItem -AccountName "ContosoADL" -Path "/MyFiles/Test.csv"
```

This command gets the details of the file Test.csv from the Data Lake Store.

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

### -Path
Specifies the Data Lake Store path from which to get details of an item, starting with the root directory (/).

```yaml
Type: DataLakeStorePathInstance
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### DataLakeStoreItem
The file or folder at the path specified.

## NOTES

## RELATED LINKS

[Export-AzureRmDataLakeStoreItem](xref:ResourceManager/AzureRM.DataLakeStore/v3.4.0/Export-AzureRmDataLakeStoreItem.md)

[Get-AzureRmDataLakeStoreChildItem](xref:ResourceManager/AzureRM.DataLakeStore/v3.4.0/Get-AzureRmDataLakeStoreChildItem.md)

[Import-AzureRmDataLakeStoreItem](xref:ResourceManager/AzureRM.DataLakeStore/v3.4.0/Import-AzureRmDataLakeStoreItem.md)

[Join-AzureRmDataLakeStoreItem](xref:ResourceManager/AzureRM.DataLakeStore/v3.4.0/Join-AzureRmDataLakeStoreItem.md)

[Move-AzureRmDataLakeStoreItem](xref:ResourceManager/AzureRM.DataLakeStore/v3.4.0/Move-AzureRmDataLakeStoreItem.md)

[New-AzureRmDataLakeStoreItem](xref:ResourceManager/AzureRM.DataLakeStore/v3.4.0/New-AzureRmDataLakeStoreItem.md)

[Remove-AzureRmDataLakeStoreItem](xref:ResourceManager/AzureRM.DataLakeStore/v3.4.0/Remove-AzureRmDataLakeStoreItem.md)

[Test-AzureRmDataLakeStoreItem](xref:ResourceManager/AzureRM.DataLakeStore/v3.4.0/Test-AzureRmDataLakeStoreItem.md)


