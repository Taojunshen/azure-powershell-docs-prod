---
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
online version: 
schema: 2.0.0
updated_at: 3/4/2017 12:37 AM
ms.date: 3/4/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/vTrue/Remove-AzureRmNetworkWatcherPacketCapture.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/vTrue/Remove-AzureRmNetworkWatcherPacketCapture.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/91cff23a000b99dc60ec82204d789c7ace1d7134/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/vTrue/Remove-AzureRmNetworkWatcherPacketCapture.md
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

# Remove-AzureRmNetworkWatcherPacketCapture

## SYNOPSIS
Removes a packet capture resource.

## SYNTAX

### SetByResource (Default)
```
Remove-AzureRmNetworkWatcherPacketCapture -NetworkWatcher <PSNetworkWatcher> -PacketCaptureName <String>
 [-PassThru] [-WhatIf] [-Confirm]
```

### SetByName
```
Remove-AzureRmNetworkWatcherPacketCapture -NetworkWatcherName <String> -ResourceGroupName <String>
 -PacketCaptureName <String> [-PassThru] [-WhatIf] [-Confirm]
```

## DESCRIPTION
The Remove-AzureRmNetworkWatcherPacketCapture removes a packet capture resource. 
It is recommended to call Stop-AzureRmNetworkWatcherPacketCapture before calling Remove-AzureRmNetworkWatcherPacketCapture. 
If the packet capture session is running when Remove-AzureRmNetworkWatcherPacketCapture is called the packet capture may not be saved. If the session is stopped prior to removal the .cap file containing capture data is not removed. 

## EXAMPLES

### --- Example 1: Remove a packet capture session --
```
Remove-AzureRmNetworkWatcherPacketCapture -NetworkWatcher $networkWatcher -PacketCaptureName "PacketCaptureTest"
```

In this example we remove an existing packet capture session named "PacketCaptureTest".

## PARAMETERS

### -NetworkWatcher
The network watcher resource.

```yaml
Type: PSNetworkWatcher
Parameter Sets: SetByResource
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -NetworkWatcherName
The name of network watcher.

```yaml
Type: String
Parameter Sets: SetByName
Aliases: Name

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -PacketCaptureName
The packet capture name.

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

### -PassThru
{{Fill PassThru Description}}

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResourceGroupName
The name of the network watcher resource group.

```yaml
Type: String
Parameter Sets: SetByName
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
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

## INPUTS

### Microsoft.Azure.Commands.Network.Models.PSNetworkWatcher
System.String

## OUTPUTS

### System.Object

## NOTES
Keywords: azure, azurerm, arm, resource, management, manager, network, networking, network watcher, packet, capture, traffic, remove

## RELATED LINKS
[New-AzureRmNetworkWatcherPacketCapture]()
[New-AzureRmPacketCaptureFilterConfig]()
[Get-AzureRmNetworkWatcherPacketCapture]()
[Stop-AzureRmNetworkWatcherPacketCapture]()

[New-AzureRmNetworkWatcher]()
[Get-AzureRmNetworkWatcher]()
[Remove-AzureRmNetworkWatcher]()

[Test-AzureRmNetworkWatcherIPFlow]()
[Get-AzureRmNetworkWatcherNextHop]()
[Get-AzureRmNetworkWatcherSecurityGroupView]()
[Get-AzureRmNetworkWatcherTopology]()
[Start-AzureRmNetworkWatcherResourceTroubleshooting]()
