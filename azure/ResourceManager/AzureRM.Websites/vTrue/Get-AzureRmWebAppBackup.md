---
external help file: Microsoft.Azure.Commands.Websites.dll-Help.xml
ms.assetid: EAAF615B-6139-438B-A2FD-6966E72B3AA9
online version: 
schema: 2.0.0
updated_at: 3/13/2017 7:40 PM
ms.date: 3/13/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ResourceManager/AzureRM.Websites/vTrue/Get-AzureRmWebAppBackup.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ResourceManager/AzureRM.Websites/vTrue/Get-AzureRmWebAppBackup.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/7201955e7e0fd9d41b0a087f20717a385bb2fb89/azureps-cmdlets-docs/ResourceManager/AzureRM.Websites/vTrue/Get-AzureRmWebAppBackup.md
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

# Get-AzureRmWebAppBackup

## SYNOPSIS
Gets the specified backup of an Azure Web App.

## SYNTAX

### FromResourceName
```
Get-AzureRmWebAppBackup [-BackupId] <String> [-ResourceGroupName] <String> [-Name] <String> [[-Slot] <String>]
 [<CommonParameters>]
```

### FromWebApp
```
Get-AzureRmWebAppBackup [-BackupId] <String> [-WebApp] <Site> [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmWebAppBackup** cmdlet gets the specified backup of an Azure Web App.

## EXAMPLES

### Example 1: Get the specified backup of an Azure Web App
```
PS C:\> Get-AzureRmWebAppBackup -ResourceGroupName "Default-Web-WestUS" -Name "WebAppStandard" -BackupId "12345"
```

This command gets the backup with ID "12345" from the Web App named WebAppStandard that belongs to the resource group Default-Web-WestUS.

## PARAMETERS

### -BackupId
Specifies the backup ID.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 3
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of the resource group.

```yaml
Type: String
Parameter Sets: FromResourceName
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Name
Specifies the name of the Web App.

```yaml
Type: String
Parameter Sets: FromResourceName
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Slot
Specifies the name of the Web App slot.

```yaml
Type: String
Parameter Sets: FromResourceName
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -WebApp
Specifies the piped WebApp.

```yaml
Type: Site
Parameter Sets: FromWebApp
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[New-AzureRmWebAppBackup](xref:ResourceManager/AzureRM.Websites/vTrue/New-AzureRmWebAppBackup.md)

[Remove-AzureRmWebAppBackup](xref:ResourceManager/AzureRM.Websites/vTrue/Remove-AzureRmWebAppBackup.md)
