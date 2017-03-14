---
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
online version: 
schema: 2.0.0
updated_at: 3/11/2017 2:20 AM
ms.date: 3/11/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v3.6.0/Set-AzureRmApplicationGatewayConnectionDraining.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v3.6.0/Set-AzureRmApplicationGatewayConnectionDraining.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04f63f6e685743ace2c57eb157574e34e8610b1c/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v3.6.0/Set-AzureRmApplicationGatewayConnectionDraining.md
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

# Set-AzureRmApplicationGatewayConnectionDraining

## SYNOPSIS
Modifies the connection draining configuration of a back-end HTTP settings object.

## SYNTAX

```
Set-AzureRmApplicationGatewayConnectionDraining -BackendHttpSettings <PSApplicationGatewayBackendHttpSettings>
 -Enabled <Boolean> -DrainTimeoutInSec <UInt32> [<CommonParameters>]
```

## DESCRIPTION
The **Set-AzureRmApplicationGatewayWebApplicationFirewallConfiguration** cmdlet modifies the connection draining configuration of a back-end HTTP settings object.

## EXAMPLES

### Example 1
```
PS C:\> $AppGw = Get-AzureRmApplicationGateway -Name "ApplicationGateway01" -ResourceGroupName "ResourceGroup01"
PS C:\> $Settings  = Get-AzureRmApplicationGatewayBackendHttpSettings -Name "Settings01" -ApplicationGateway $AppGw
PS C:\> Set-AzureRmApplicationGatewayConnectionDraining -BackendHttpSettings $poolSetting02 -Enabled $False -DrainTimeoutInSec 3600
```

The first command gets the application gateway named ApplicationGateway01 in the resource group named ResourceGroup01 and stores it in the $AppGw variable.
The second command gets the back-end HTTP settings named Settings01 for $AppGw and stores the settings in the $Settings variable.
The last command modifies the connection draining configuration of the back-end HTTP settings object stored in $Settings by setting Enabled to False and DrainTimeoutInSec to 3600.

## PARAMETERS

### -BackendHttpSettings
The backend http settings

```yaml
Type: PSApplicationGatewayBackendHttpSettings
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -DrainTimeoutInSec
The number of seconds connection draining is active.
Acceptable values are from 1 second to 3600 seconds.

```yaml
Type: UInt32
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Enabled
Whether connection draining is enabled or not.

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Azure.Commands.Network.Models.PSApplicationGatewayBackendHttpSettings

## OUTPUTS

### Microsoft.Azure.Commands.Network.Models.PSApplicationGatewayBackendHttpSettings

## NOTES

## RELATED LINKS

[Get-AzureRmApplicationGateway](xref:ResourceManager/AzureRM.Network/v3.6.0/Get-AzureRmApplicationGateway.md)

[Get-AzureRmApplicationGatewayBackendHttpSettings](xref:ResourceManager/AzureRM.Network/v3.6.0/Get-AzureRmApplicationGatewayBackendHttpSettings.md)

[Get-AzureRmApplicationGatewayConnectionDraining](xref:ResourceManager/AzureRM.Network/v3.6.0/Get-AzureRmApplicationGatewayConnectionDraining.md)

[New-AzureRmApplicationGatewayConnectionDraining](xref:ResourceManager/AzureRM.Network/v3.6.0/New-AzureRmApplicationGatewayConnectionDraining.md)

[Remove-AzureRmApplicationGatewayConnectionDraining](xref:ResourceManager/AzureRM.Network/v3.6.0/Remove-AzureRmApplicationGatewayConnectionDraining.md)

