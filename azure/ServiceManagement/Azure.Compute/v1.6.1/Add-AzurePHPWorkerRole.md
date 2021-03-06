---
external help file: Microsoft.WindowsAzure.Commands.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 4759CE95-BB7A-46F0-8125-2A1966F572D4
updated_at: 11/18/2016 11:58 PM
ms.date: 11/18/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Compute/v1.6.1/Add-AzurePHPWorkerRole.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Compute/v1.6.1/Add-AzurePHPWorkerRole.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/72a3aea1f1ed5e83ed5c6c8596a219daeabbbe22/azureps-cmdlets-docs/ServiceManagement/Azure.Compute/v1.6.1/Add-AzurePHPWorkerRole.md
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

# Add-AzurePHPWorkerRole

## SYNOPSIS
Creates the required files and configuration (sometimes referred to as scaffolding) for a PHP application that will be hosted in Azure through php.exe.

## SYNTAX

```
Add-AzurePHPWorkerRole [[-Name] <String>] [[-Instances] <Int32>] [-Profile <AzureSMProfile>]
 [<CommonParameters>]
```

## DESCRIPTION
powershell_prelim

Creates the required files and configuration (sometimes referred to as scaffolding) for a PHP application that will be hosted in Azure through php.exe.

## EXAMPLES

### 1: Create a worker role with a single instance
```
PS C:\>Add-AzurePHPWorkerRole MyWorkerRole
```

This example adds the required files and configuration for a single worker role named "MyWorkerRole" to the current application.

### 2: Create a worker role with multiple instances
```
PS C:\>Add-AzurePHPWorkerRole MyWorkerRole -I 2
```

This example adds the required files and configuration for a new worker role to the current application, using the name "MyWorkerRole" with a role instance count of 2.

## PARAMETERS

### -Name
Specifies the name of the worker role.
The name determines the folder name that contains the required files and configuration for the PHP service hosted in the worker role.
The default is WorkerRole1.

```yaml
Type: String
Parameter Sets: (All)
Aliases: n

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Instances
Specifies the number of role instances for this worker role.
The default is 1.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: i

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Profile
In-memory profile.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[New-AzureServiceProject](xref:ServiceManagement/Azure.Compute/v1.6.1/New-AzureServiceProject.md)

[Add-AzurePHPWebRole](xref:ServiceManagement/Azure.Compute/v1.6.1/Add-AzurePHPWebRole.md)


