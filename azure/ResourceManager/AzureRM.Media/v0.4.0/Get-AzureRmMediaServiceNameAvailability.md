---
external help file: Microsoft.Azure.Commands.Media.dll-Help.xml
ms.assetid: 23C6C9D3-A745-46C8-AB2C-B874223FBFFF
online version: 
schema: 2.0.0
updated_at: 3/11/2017 2:20 AM
ms.date: 3/11/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Media/v0.4.0/Get-AzureRmMediaServiceNameAvailability.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Media/v0.4.0/Get-AzureRmMediaServiceNameAvailability.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04f63f6e685743ace2c57eb157574e34e8610b1c/azureps-cmdlets-docs/ResourceManager/AzureRM.Media/v0.4.0/Get-AzureRmMediaServiceNameAvailability.md
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

# Get-AzureRmMediaServiceNameAvailability

## SYNOPSIS
Checks whether a media service name is available.
Media service names are globally unique.

## SYNTAX

```
Get-AzureRmMediaServiceNameAvailability [-AccountName] <String> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmMediaServiceNameAvailability** cmdlet checks whether a media service name is available.
Media service names are globally unique.

## EXAMPLES

### Example 1: Check whether a Media Service name is available
```
PS C:\>Get-AzureRmMediaServiceNameAvailability -AccountName "MediaService1"
```

This command checks if the name MediaService1 is available.

## PARAMETERS

### -AccountName
Specifies the name of the media service that this cmdlet gets.

```yaml
Type: String
Parameter Sets: (All)
Aliases: Name, ResourceName

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationAction
Specifies how this cmdlet responds to an information event.

The acceptable values for this parameter are:

- Continue
- Ignore
- Inquire
- SilentlyContinue
- Stop
- Suspend

```yaml
Type: ActionPreference
Parameter Sets: (All)
Aliases: infa

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationVariable
Specifies an information variable.

```yaml
Type: String
Parameter Sets: (All)
Aliases: iv

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

[Get-AzureRmMediaService](xref:ResourceManager/AzureRM.Media/v0.4.0/Get-AzureRmMediaService.md)

[New-AzureRmMediaService](xref:ResourceManager/AzureRM.Media/v0.4.0/New-AzureRmMediaService.md)

[Remove-AzureRmMediaService](xref:ResourceManager/AzureRM.Media/v0.4.0/Remove-AzureRmMediaService.md)

[Set-AzureRmMediaService](xref:ResourceManager/AzureRM.Media/v0.4.0/Set-AzureRmMediaService.md)


