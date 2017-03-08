---
external help file: Microsoft.Azure.Commands.DataLakeStore.dll-Help.xml
online version: 
schema: 2.0.0
updated_at: 3/4/2017 9:58 PM
ms.date: 3/4/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ResourceManager/AzureRM.DataLakeStore/v3.3.0/Set-AzureRmDataLakeStoreItemExpiry.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ResourceManager/AzureRM.DataLakeStore/v3.3.0/Set-AzureRmDataLakeStoreItemExpiry.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/7761f732d57261bdc233763ac2d243d320e93043/azureps-cmdlets-docs/ResourceManager/AzureRM.DataLakeStore/v3.3.0/Set-AzureRmDataLakeStoreItemExpiry.md
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

# Set-AzureRmDataLakeStoreItemExpiry

## SYNOPSIS
Sets or removes the expire time for a file in an Azure Data Lake Store account.

## SYNTAX

```
Set-AzureRmDataLakeStoreItemExpiry [-Account] <String> [-Path] <DataLakeStorePathInstance>
 [[-Expiration] <DateTimeOffset>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The Set-AzureRmDataLakeStoreItemExpiry cmdlet sets or removes the expire time for a file in an Azure Data Lake Store account.

## EXAMPLES

### Example 1: Set the expiration time for a file
```
PS C:\> Set-AzureRmDataLakeStoreItemExpiry -AccountName "ContosoADL" -Path /myfile.txt -Expiration [DateTimeOffset]::Now.AddHours(2)
```

This command sets expiration on the file myfile.txt in account ContosoADL to be two hours from now.
This will cause the file to expire (be marked for delete) in two hours.

### Example 2: Remove the expiration on a file
```
PS C:\> Set-AzureRmDataLakeStoreItemExpiry -AccountName "ContosoADL" -Path /myfile.txt
```

This command removes any expiration that was previously set on file myfile.txt in the account named ContosoADL.
The file will not automatically expire (be marked for delete) and needs to be manually deleted or set to expire again.

## PARAMETERS

### -Account
Specifies the Data Lake Store account name.

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

### -Expiration
Specifies the absolute expiration time for the specified file.
If no value or set to MaxValue, the file will never expire.

```yaml
Type: DateTimeOffset
Parameter Sets: (All)
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Path
Specifies the Data Lake Store path of the file item for which to set or remove expiry.

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
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

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

### Microsoft.Azure.Commands.DataLakeStore.Models.DataLakeStoreItem

## NOTES
Alias: Set-AdlStoreItemExpiry

## RELATED LINKS

[Get-AzureRmDataLakeStoreItem](xref:ResourceManager/AzureRM.DataLakeStore/v3.3.0/Get-AzureRmDataLakeStoreItem.md)
