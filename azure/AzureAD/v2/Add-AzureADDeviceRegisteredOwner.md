---
external help file: Microsoft.Open.AzureAD16.Graph.PowerShell.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 31B92E0F-E46C-4371-8AC9-6C2B497C979B
updated_at: 11/2/2016 12:03 AM
ms.date: 11/2/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/master/Azure%20AD%20Cmdlets/AzureAD/v2/Add-AzureADDeviceRegisteredOwner.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/2a11b877460cc9035f1d8a73f7be908047b47fb5/Azure%20AD%20Cmdlets/AzureAD/v2/Add-AzureADDeviceRegisteredOwner.md
ms.topic: reference
ms.prod: powershell
ms.service: Azure PowerShell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Add-AzureADDeviceRegisteredOwner

## SYNOPSIS
Adds a registered owner for a device.
## SYNTAX

```
Add-AzureADDeviceRegisteredOwner -ObjectId <String> -RefObjectId <String> [<CommonParameters>]
```

## DESCRIPTION
The **Add-AzureADDeviceRegisteredOwner** cmdlet adds a registerd owner for an Azure Active Directory device.
## EXAMPLES

## PARAMETERS

### -ObjectId
Specifies the object ID. 
```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -RefObjectId
Specifies the ID of the Active Directory object to add.
```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS
[Get-AzureADDeviceRegisteredOwner](.\Get-AzureADDeviceRegisteredOwner)

[Remove-AzureADDeviceRegisteredOwner](.\Remove-AzureADDeviceRegisteredOwner)