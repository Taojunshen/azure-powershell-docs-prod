---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.dll-Help.xml
online version: .\Get-AzureDataDisk.md
schema: 2.0.0
ms.assetid: AD3170AB-3678-4AA7-BCA2-04EA7AE2A0EC
updated_at: 10/18/2016 9:38 PM
ms.date: 10/18/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v2.1.0/Get-AzureOSDisk.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/23cdb8705d4ab9807c0e21b238f3b134a7d49c7d/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v2.1.0/Get-AzureOSDisk.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AzureOSDisk

## SYNOPSIS
Gets the operating system disk of an Azure virtual machine.

## SYNTAX

```
Get-AzureOSDisk -VM <IPersistentVM> [-Profile <AzureSMProfile>] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureOSDisk** cmdlet gets the operating system disk of an Azure virtual machine.

## EXAMPLES

### Example 1: Get an operating system disk
```
PS C:\>Get-AzureVM -ServiceName "ContosoService" -Name "VirtualMachine02" | Get-AzureOSDisk
```

This command gets the virtual machine named VirtualMachine02 in the service named ContosoService by using the **Get-AzureVM** cmdlet.
The command passes the virtual machine to the current cmdlet by using the pipeline operator.
The current cmdlet gets the operating system disk of that virtual machine.

## PARAMETERS

### -VM
Specifies the virtual machine for which this cmdlet gets the operating system disk.
To obtain a virtual machine object, use the Get-AzureVM cmdlet.

```yaml
Type: IPersistentVM
Parameter Sets: (All)
Aliases: InputObject

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
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

### -InformationAction
@{Text=}```yaml
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
@{Text=}```yaml
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

[Get-AzureDataDisk](.\Get-AzureDataDisk.md)

[Set-AzureOSDisk](.\Set-AzureOSDisk.md)

