---
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
ms.assetid: F0370845-13D9-4FB5-B30E-826A22EBC5E0
online version:
schema: 2.0.0
updated_at: 3/10/2017 7:40 PM
ms.date: 3/10/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/vTrue/Get-AzureRmExpressRouteCircuitARPTable.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/vTrue/Get-AzureRmExpressRouteCircuitARPTable.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/16665bd43882b185a8143de54e498a0463907aa7/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/vTrue/Get-AzureRmExpressRouteCircuitARPTable.md
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

# Get-AzureRmExpressRouteCircuitARPTable

## SYNOPSIS

Gets the ARP table from an ExpressRoute circuit.

## SYNTAX

```
Get-AzureRmExpressRouteCircuitARPTable -ResourceGroupName <String> -ExpressRouteCircuitName
 <String> [-PeeringType <String>] -DevicePath <DevicePathEnum> [-InformationAction
 <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION

The **Get-AzureRmExpressRouteCircuitARPTable** cmdlet retrieves the ARP table from both interfaces
of an ExpressRoute circuit. The ARP table provides a mapping of the IPv4 address to MAC address for
a particular peering. You can use the ARP table to validate layer 2 configuration and connectivity.

## EXAMPLES

### Example 1: Display the ARP table for an ExpressRoute peer

```powershell
Get-AzureRmExpressRouteCircuitARPTable -ResourceGroupName $RG -ExpressRouteCircuitName $CircuitName -PeeringType MicrosoftPeering -DevicePath Primary
```

## PARAMETERS

### -ResourceGroupName

The name of the resource group containing the ExpressRoute circuit.

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

### -ExpressRouteCircuitName

The name of the ExpressRoute circuit being examined.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -PeeringType

The acceptable values for this parameter are: `AzurePrivatePeering`, `AzurePublicPeering`, and
`MicrosoftPeering`

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

### -DevicePath

The acceptable values for this parameter are: `Primary` or `Secondary`

```yaml
Type: DevicePathEnum
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
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

This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable,
-InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose,
-WarningAction, and -WarningVariable. For more information, see about_CommonParameters
(http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureRmExpressRouteCircuitRouteTable](Get-AzureRmExpressRouteCircuitRouteTable.md)

[Get-AzureRmExpressRouteCircuitRouteTableSummary](Get-AzureRmExpressRouteCircuitRouteTableSummary.md)

[Get-AzureRmExpressRouteCircuitStats](Get-AzureRmExpressRouteCircuitStats.md)
