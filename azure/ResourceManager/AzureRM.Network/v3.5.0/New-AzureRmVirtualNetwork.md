---
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
ms.assetid: 81D55C43-C9A3-4DA7-A469-A3A7550FE9A4
online version: 
schema: 2.0.0
updated_at: 3/11/2017 3:58 PM
ms.date: 3/11/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v3.5.0/New-AzureRmVirtualNetwork.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v3.5.0/New-AzureRmVirtualNetwork.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/bc71000aa3c7f754b95442dcc415a7324626a15c/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v3.5.0/New-AzureRmVirtualNetwork.md
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

# New-AzureRmVirtualNetwork

## SYNOPSIS
Creates a virtual network.

## SYNTAX

```
New-AzureRmVirtualNetwork -Name <String> -ResourceGroupName <String> -Location <String>
 -AddressPrefix <System.Collections.Generic.List`1[System.String]>
 [-DnsServer <System.Collections.Generic.List`1[System.String]>]
 [-Subnet <System.Collections.Generic.List`1[Microsoft.Azure.Commands.Network.Models.PSSubnet]>]
 [-Tag <Hashtable>] [-Force] [-InformationAction <ActionPreference>] [-InformationVariable <String>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The **New-AzureRmVirtualNetwork** cmdlet creates an Azure virtual network.

## EXAMPLES

### 1:
```
 New-AzureRmResourceGroup -Name TestResourceGroup -Location centralus
    $frontendSubnet = New-AzureRmVirtualNetworkSubnetConfig -Name frontendSubnet 
    -AddressPrefix "10.0.1.0/24"
    $backendSubnet = New-AzureRmVirtualNetworkSubnetConfig -Name backendSubnet -AddressPrefix 
    "10.0.2.0/24"
    New-AzureRmVirtualNetwork -Name MyVirtualNetwork -ResourceGroupName TestResourceGroup 
    -Location centralus -AddressPrefix "10.0.0.0/16" -Subnet $frontendSubnet,$backendSubnet
```
This example creates a virtual network with two subnets. First, a new resource group is 
    created in the centralus region. Then, the example creates in-memory representations of 
    two subnets. The New-AzureRmVirtualNetworkSubnetConfig cmdlet will not create any subnet 
    on the server side. There is one subnet called frontendSubnet and one subnet called 
    backendSubnet. The New-AzureRmVirtualNetwork cmdlet then creates a virtual network using 
    the CIDR 10.0.0.0/16 as the address prefix and two subnets.
### 2:  Create a virtual network with DNS settings 
```
New-AzureRmResourceGroup -Name TestResourceGroup -Location centralus
    $frontendSubnet = New-AzureRmVirtualNetworkSubnetConfig -Name frontendSubnet 
    -AddressPrefix "10.0.1.0/24"
    $backendSubnet = New-AzureRmVirtualNetworkSubnetConfig -Name backendSubnet -AddressPrefix 
    "10.0.2.0/24"
    New-AzureRmVirtualNetwork -Name MyVirtualNetwork -ResourceGroupName TestResourceGroup 
    -Location centralus -AddressPrefix "10.0.0.0/16" -Subnet $frontendSubnet,$backendSubnet 
    -DnsServer 10.0.1.5,10.0.1.6
```
This example create a virtual network with two subnets and two DNS servers. The effect of 
    specifying the DNS servers on the virtual network is that the NICs/VMs that are deployed 
    into this virtual network inherit these DNS servers as defaults. These defaults can be 
    overwritten per NIC through a NIC-level setting. If no DNS servers are specified on a 
    VNET and no DNS servers on the NICs, then the default Azure DNS servers are used for DNS 
    resolution.
### 3: Create a virtual network with a subnet referencing a network security group
```
New-AzureRmResourceGroup -Name TestResourceGroup -Location centralus
    $rdpRule = New-AzureRmNetworkSecurityRuleConfig -Name rdp-rule -Description "Allow RDP" 
    -Access Allow -Protocol Tcp -Direction Inbound -Priority 100 -SourceAddressPrefix 
    Internet -SourcePortRange * -DestinationAddressPrefix * -DestinationPortRange 3389
    $networkSecurityGroup = New-AzureRmNetworkSecurityGroup -ResourceGroupName 
    TestResourceGroup -Location centralus -Name "NSG-FrontEnd" -SecurityRules $rdpRule
    $frontendSubnet = New-AzureRmVirtualNetworkSubnetConfig -Name frontendSubnet 
    -AddressPrefix "10.0.1.0/24" -NetworkSecurityGroup $networkSecurityGroup
    $backendSubnet = New-AzureRmVirtualNetworkSubnetConfig -Name backendSubnet -AddressPrefix 
    "10.0.2.0/24" -NetworkSecurityGroup $networkSecurityGroup
    New-AzureRmVirtualNetwork -Name MyVirtualNetwork -ResourceGroupName TestResourceGroup 
    -Location centralus -AddressPrefix "10.0.0.0/16" -Subnet $frontendSubnet,$backendSubnet
```
 This example creates a virtual network with subnets that reference a network security 
    group. First, the example creates a resource group as a container for the resources that 
    will be created. Then, a network security group is created that allows inbound RDP 
    access, but otherwise enforces the default network security group rules. The 
    New-AzureRmVirtualNetworkSubnetConfig cmdlet then creates in-memory representations of 
    two subnets that both reference the network security group that was created. The 
    New-AzureRmVirtualNetwork command then creates the virtual network.

## PARAMETERS

### -Name
Specifies the name of the virtual network that this cmdlet creates.

```yaml
Type: String
Parameter Sets: (All)
Aliases: ResourceName

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of a resource group to contain the virtual network.

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

### -Location
Specifies the region for the virtual network.

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

### -AddressPrefix
Specifies a range of IP addresses for a virtual network.

```yaml
Type: System.Collections.Generic.List`1[System.String]
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -DnsServer
Specifies the DNS server for a subnet.

```yaml
Type: System.Collections.Generic.List`1[System.String]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Subnet
Specifies a list of subnets to associate with the virtual network.

```yaml
Type: System.Collections.Generic.List`1[Microsoft.Azure.Commands.Network.Models.PSSubnet]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Tag
Specifies a dictionary of tags to associate with the network interface.

```yaml
Type: Hashtable
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Force
Forces the command to run without asking for user confirmation.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureRmVirtualNetwork](xref:ResourceManager/AzureRM.Network/v3.5.0/Get-AzureRmVirtualNetwork.md)

[Remove-AzureRmVirtualNetwork](xref:ResourceManager/AzureRM.Network/v3.5.0/Remove-AzureRmVirtualNetwork.md)

[Set-AzureRmVirtualNetwork](xref:ResourceManager/AzureRM.Network/v3.5.0/Set-AzureRmVirtualNetwork.md)


