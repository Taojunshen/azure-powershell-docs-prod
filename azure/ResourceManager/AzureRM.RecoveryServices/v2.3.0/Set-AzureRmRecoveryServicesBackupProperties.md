---
external help file: Microsoft.Azure.Commands.RecoveryServices.ARM.dll-Help.xml
ms.assetid: FBA2DBFB-F9C1-4C19-8DE3-A9CA50EB72B3
online version: 
schema: 2.0.0
updated_at: 11/8/2016 12:38 AM
ms.date: 11/8/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.RecoveryServices/v2.3.0/Set-AzureRmRecoveryServicesBackupProperties.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04b9ae2d1c44a3ada330f570237886794cede893/azureps-cmdlets-docs/ResourceManager/AzureRM.RecoveryServices/v2.3.0/Set-AzureRmRecoveryServicesBackupProperties.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Set-AzureRmRecoveryServicesBackupProperties

## SYNOPSIS
Sets the properties for backup management.

## SYNTAX

```
Set-AzureRmRecoveryServicesBackupProperties -Vault <ARSVault>
 [-BackupStorageRedundancy <AzureRmRecoveryServicesBackupStorageRedundancyType>] [<CommonParameters>]
```

## DESCRIPTION
The **Set-AzureRmRecoveryServicesBackupProperties** cmdlet sets backup storage properties for a Recovery Services vault.

## EXAMPLES

### Example 1: Set GeoRedundant storage for a vault
```
PS C:\> $Vault01 = Get-AzureRmRecoveryServicesVault -Name "TestVault"
PS C:\> Set-AzureRmRecoveryServicesBackupProperties -Vault $Vault01 -BackupStorageRedundancy GeoRedundant
```

The first command gets the vault named TestVault, and then stores it in the $Vault01 variable.

The second command sets the backup storage redundancy for $Vault01 to GeoRedundant.

## PARAMETERS

### -Vault
Specifies the name of the vault.
The vault must be an **AzureRmRecoveryServicesVault** object.

```yaml
Type: ARSVault
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -BackupStorageRedundancy
Specifies the backup storage redundancy type.

```yaml
Type: AzureRmRecoveryServicesBackupStorageRedundancyType
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

[Get-AzureRmRecoveryServicesBackupProperties](xref:ResourceManager/AzureRM.RecoveryServices/v2.3.0/Get-AzureRmRecoveryServicesBackupProperties.md)

[Get-AzureRmRecoveryServicesVault](xref:ResourceManager/AzureRM.RecoveryServices/v2.3.0/Get-AzureRmRecoveryServicesVault.md)

