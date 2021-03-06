---
external help file: Microsoft.Azure.Commands.Compute.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: DB6ADAFB-2FF2-4BE8-9284-DBE399D87890
updated_at: 11/11/2016 11:03 PM
ms.date: 11/11/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Compute/v2.2.0/New-AzureRmContainerService.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Compute/v2.2.0/New-AzureRmContainerService.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/79eeb985ea480979357fb4695832a0c3d29a48bf/azureps-cmdlets-docs/ResourceManager/AzureRM.Compute/v2.2.0/New-AzureRmContainerService.md
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

# New-AzureRmContainerService

## SYNOPSIS
Creates a container service.

## SYNTAX

```
New-AzureRmContainerService [-WhatIf] [-Confirm] [-ResourceGroupName] <String> [-Name] <String>
 [-ContainerService] <ContainerService> [<CommonParameters>]
```

## DESCRIPTION
The **New-AzureRmContainerService** cmdlet creates a container service.
Specify a container service object that you can create by using the New-AzureRmContainerServiceConfig cmdlet.

## EXAMPLES

### Example 1: Create a container service
```
PS C:\>New-AzureRMResourceGroup -Name "ResourceGroup17" -Location "Australia Southeast" -Force
PS C:\> $Container = New-AzureRmContainerServiceConfig -Location "Australia Southeast" -OrchestratorType "DCOS" -MasterDnsPrefix "MasterResourceGroup17" -AdminUsername "AcsLinuxAdmin" -SshPublicKey "<ssh-key>" | Add-AzureRmContainerServiceAgentPoolProfile -Name "AgentPool01" -VmSize "Standard_A1" -DnsPrefix "APResourceGroup17"
PS C:\> New-AzureRmContainerService -ResourceGroupName "ResourceGroup17" -Name "CSResourceGroup17" -ContainerService $Container
```

The first command creates a resource group named ResourceGroup17 at the specified location.
For more information, see the New-AzureRmResourceGroup cmdlet.

The second command creates a container, and then stores it in the $Container variable.
For more information, see the New-AzureRmContainerServiceConfig cmdlet.

The final command creates a container service for the container stored in $Container.
The service is named csResourceGroup17.

## PARAMETERS

### -ContainerService
Specifies a container service object that contains the properties for the new service.
To obtain a **ContainerService** object, use the New-AzureRmContainerServiceConfig cmdlet.

```yaml
Type: ContainerService
Parameter Sets: (All)
Aliases: 

Required: True
Position: 4
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Name
Specifies the name of the container service that this cmdlet creates.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the resource group in which this cmdlet deploys the container service.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
Default value: None
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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureRmContainerService](xref:ResourceManager/AzureRM.Compute/v2.2.0/Get-AzureRmContainerService.md)

[New-AzureRmContainerServiceConfig](xref:ResourceManager/AzureRM.Compute/v2.2.0/New-AzureRmContainerServiceConfig.md)

[Remove-AzureRmContainerService](xref:ResourceManager/AzureRM.Compute/v2.2.0/Remove-AzureRmContainerService.md)

[Update-AzureRmContainerService](xref:ResourceManager/AzureRM.Compute/v2.2.0/Update-AzureRmContainerService.md)


