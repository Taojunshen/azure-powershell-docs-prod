---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.Network.dll-Help.xml
ms.assetid: 5765F6BD-38BC-451B-85C5-F5D1A5AF2831
online version: 
schema: 2.0.0
updated_at: 1/20/2017 9:17 PM
ms.date: 1/20/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Networking/v3.4.0/Resize-AzureVNetGateway.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Networking/v3.4.0/Resize-AzureVNetGateway.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/cb06bb906911a2a2e1f57adbafe0c0c97a0b205b/azureps-cmdlets-docs/ServiceManagement/Azure.Networking/v3.4.0/Resize-AzureVNetGateway.md
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

# Resize-AzureVNetGateway

## SYNOPSIS
Resizes a VPN gateway.

## SYNTAX

```
Resize-AzureVNetGateway -VNetName <String> -GatewaySKU <String> [-Profile <AzureSMProfile>]
 [<CommonParameters>]
```

## DESCRIPTION
The **Resize-AzureVNetGateway** cmdlet resizes a virtual network virtual private network (VPN) gateway to a different SKU.
Valid SKUs for a virtual network gateway are Default, Standard, and HighPerformance.

## EXAMPLES

### Example 1: Change the SKU for a virtual network gateway
```
PS C:\> Resize-AzureVNetGateway -VNetName "ContosoVN07" -GatewaySKU "HighPerformance"
```

This command changes the SKU of the virtual network gateway for the virtual network named ContosoVN07 to HighPerformance.

## PARAMETERS

### -GatewaySKU
Specifies the SKU to which this cmdlet resizes virtual network gateway.
Valid values are: 

- Default 
- Standard 
- HighPerformance

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Profile
Specifies the Azure profile from which this cmdlet reads. 
If you do not specify a profile, this cmdlet reads from the local default profile.

```yaml
Type: AzureSMProfile
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -VNetName
Specifies the virtual network in which this cmdlet resizes a virtual network gateway.

```yaml
Type: String
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

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureVNetGateway](xref:ServiceManagement/Azure.Networking/v3.4.0/Get-AzureVNetGateway.md)

[New-AzureVNetGateway](xref:ServiceManagement/Azure.Networking/v3.4.0/New-AzureVNetGateway.md)

[Remove-AzureVNetGateway](xref:ServiceManagement/Azure.Networking/v3.4.0/Remove-AzureVNetGateway.md)

[Reset-AzureVNetGateway](xref:ServiceManagement/Azure.Networking/v3.4.0/Reset-AzureVNetGateway.md)

[Set-AzureVNetGatewayKey](xref:ServiceManagement/Azure.Networking/v3.4.0/Set-AzureVNetGatewayKey.md)


