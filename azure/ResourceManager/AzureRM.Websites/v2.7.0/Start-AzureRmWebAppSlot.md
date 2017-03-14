---
external help file: Microsoft.Azure.Commands.Websites.dll-Help.xml
ms.assetid: 0FDDDEE1-CEAD-46DA-A7EB-EE477ED59749
online version: 
schema: 2.0.0
updated_at: 3/11/2017 2:20 AM
ms.date: 3/11/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ResourceManager/AzureRM.Websites/v2.7.0/Start-AzureRmWebAppSlot.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ResourceManager/AzureRM.Websites/v2.7.0/Start-AzureRmWebAppSlot.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04f63f6e685743ace2c57eb157574e34e8610b1c/azureps-cmdlets-docs/ResourceManager/AzureRM.Websites/v2.7.0/Start-AzureRmWebAppSlot.md
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

# Start-AzureRmWebAppSlot

## SYNOPSIS
Starts an Azure Web App slot.

## SYNTAX

### S1
```
Start-AzureRmWebAppSlot [-ResourceGroupName] <String> [-Name] <String> [-Slot] <String>
```

### S2
```
Start-AzureRmWebAppSlot [-WebApp] <Site>
```

## DESCRIPTION
The **Start-AzureRmWebAppSlot** cmdlet starts an Azure Web App Slot.

## EXAMPLES

### Example 1
```
PS C:\>Start-AzureRmWebAppSlot -ResourceGroupName "Default-Web-WestUS" -Name "ContosoWebApp" -Slot "Slot001"
```

This command starts the Slot named Slot001 pertaining to the Web App named ContosoWebApp that belongs to the resource group named Default-Web-WestUS.

## PARAMETERS

### -Name
WebApp Name

```yaml
Type: String
Parameter Sets: S1
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Resource Group Name

```yaml
Type: String
Parameter Sets: S1
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Slot
WebApp Slot Name

```yaml
Type: String
Parameter Sets: S1
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WebApp
WebApp Object

```yaml
Type: Site
Parameter Sets: S2
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureRMWebAppSlot](xref:ResourceManager/AzureRM.Websites/v2.7.0/Get-AzureRMWebAppSlot.md)

[New-AzureRMWebAppSlot](xref:ResourceManager/AzureRM.Websites/v2.7.0/New-AzureRMWebAppSlot.md)

[Remove-AzureRMWebAppSlot](xref:ResourceManager/AzureRM.Websites/v2.7.0/Remove-AzureRMWebAppSlot.md)

[Restart-AzureRMWebAppSlot](xref:ResourceManager/AzureRM.Websites/v2.7.0/Restart-AzureRMWebAppSlot.md)

[Set-AzureRMWebAppSlot](xref:ResourceManager/AzureRM.Websites/v2.7.0/Set-AzureRMWebAppSlot.md)

[Stop-AzureRMWebAppSlot](xref:ResourceManager/AzureRM.Websites/v2.7.0/Stop-AzureRMWebAppSlot.md)

[Get-AzureRmWebApp](xref:ResourceManager/AzureRM.Websites/v2.7.0/Get-AzureRmWebApp.md)
