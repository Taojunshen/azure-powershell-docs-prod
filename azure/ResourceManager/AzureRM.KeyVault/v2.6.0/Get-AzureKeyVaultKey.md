---
external help file: Microsoft.Azure.Commands.KeyVault.dll-Help.xml
ms.assetid: 2BE34AE1-06FA-4F66-8FDB-CED22C2E0978
online version: http://go.microsoft.com/fwlink/?LinkId=690297
schema: 2.0.0
updated_at: 3/11/2017 3:58 PM
ms.date: 3/11/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.KeyVault/v2.6.0/Get-AzureKeyVaultKey.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.KeyVault/v2.6.0/Get-AzureKeyVaultKey.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/bc71000aa3c7f754b95442dcc415a7324626a15c/azureps-cmdlets-docs/ResourceManager/AzureRM.KeyVault/v2.6.0/Get-AzureKeyVaultKey.md
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

# Get-AzureKeyVaultKey

## SYNOPSIS
Gets Key Vault keys.

## SYNTAX

### ByVaultName (Default)
```
Get-AzureKeyVaultKey [-VaultName] <String> [<CommonParameters>]
```

### ByKeyName
```
Get-AzureKeyVaultKey [-VaultName] <String> [-Name] <String> [[-Version] <String>] [<CommonParameters>]
```

### ByKeyVersions
```
Get-AzureKeyVaultKey [-VaultName] <String> [-Name] <String> [-IncludeVersions] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureKeyVaultKey** cmdlet gets Azure Key Vault keys.
This cmdlet gets a specific **Microsoft.Azure.Commands.KeyVault.Models.KeyBundle** or a list of all **KeyBundle** objects in a key vault or by version.

## EXAMPLES

### Example 1: Get all the keys in a key vault
```
PS C:\>Get-AzureKeyVaultKey -VaultName 'Contoso'
```

This command gets all the keys in the key vault named Contoso.

### Example 2: Get the current version of a key
```
PS C:\>Get-AzureKeyVaultKey -VaultName 'Contoso' -KeyName 'ITPfx'
```

This command gets the current version of the key named ITPfx in the key vault named Contoso.

### Example 3: Get all versions of a key
```
PS C:\>Get-AzureKeyVaultKey -VaultName 'Contoso' -KeyName 'ITPfx' -IncludeVersions
```

This command gets all versions the key named ITPfx in the key vaultnamed Contoso.

### Example 4: Get a specific version of a key
```
PS C:\>$Key = Get-AzureKeyVaultKey -VaultName 'Contoso' -KeyName 'ITPfx' -Version '5A12A276385949DB8B5F82AFEE85CAED'
```

This command gets a specific version of the key named ITPfx in the key vault named Contoso.
After running this command, you can inspect various properties of the key by navigating the $Key object.

## PARAMETERS

### -IncludeVersions
Indicates that this cmdlet gets all versions of a key.
The current version of a key is the first one on the list.
If you specify this parameter you must also specify the *Name* and *VaultName* parameters.

If you do not specify the *IncludeVersions* parameter, this cmdlet gets the current version of the key with the specified *Name*.

```yaml
Type: SwitchParameter
Parameter Sets: ByKeyVersions
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
Specifies the name of the key bundle to get.

```yaml
Type: String
Parameter Sets: ByKeyName, ByKeyVersions
Aliases: KeyName

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -VaultName
Specifies the name of the key vault from which this cmdlet gets keys.
This cmdlet constructs the fully qualified domain name (FQDN) of a key vault based on the name that this parameter specifies and your selected environment.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Version
Specifies the key version.
This cmdlet constructs the FQDN of a key based on the key vault name, your currently selected environment, the key name, and the key version.

```yaml
Type: String
Parameter Sets: ByKeyName
Aliases: KeyVersion

Required: False
Position: 3
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### String

## OUTPUTS

### List<Microsoft.Azure.Commands.KeyVault.Models.KeyBundle>, Microsoft.Azure.Commands.KeyVault.Models.KeyBundle

## NOTES

## RELATED LINKS

[Add-AzureKeyVaultKey](xref:ResourceManager/AzureRM.KeyVault/v2.6.0/Add-AzureKeyVaultKey.md)

[Remove-AzureKeyVaultKey](xref:ResourceManager/AzureRM.KeyVault/v2.6.0/Remove-AzureKeyVaultKey.md)

[Set-AzureKeyVaultKeyAttribute](xref:ResourceManager/AzureRM.KeyVault/v2.6.0/Set-AzureKeyVaultKeyAttribute.md)

