---
external help file: Microsoft.Azure.Commands.KeyVault.dll-Help.xml

online version: http://go.microsoft.com/fwlink/?LinkId=690300
schema: 2.0.0
updated_at: 3/11/2017 3:58 PM
ms.date: 3/11/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.KeyVault/v2.6.0/Remove-AzureKeyVaultSecret.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.KeyVault/v2.6.0/Remove-AzureKeyVaultSecret.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/bc71000aa3c7f754b95442dcc415a7324626a15c/azureps-cmdlets-docs/ResourceManager/AzureRM.KeyVault/v2.6.0/Remove-AzureKeyVaultSecret.md
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

# Remove-AzureKeyVaultSecret

## SYNOPSIS
Deletes a secret in a key vault.

## SYNTAX

```
Remove-AzureKeyVaultSecret [-VaultName] <String> [-Name] <String> [-Force] [-PassThru] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

## DESCRIPTION
The Remove-AzureKeyVaultSecret cmdlet deletes a secret in a key vault.
This cmdlet has a value of high for the **ConfirmImpact** property.

## EXAMPLES

### Example 1: Remove a secret from a key vault
```
PS C:\>Remove-AzureKeyVaultSecret -VaultName 'Contoso' -Name 'FinanceSecret'
```

This command removes the secret named FinanceSecret from the key vault named Contoso.'

### Example 2: Remove a secret from a key vault without user confirmation
```
PS C:\>Remove-AzureKeyVaultSecret -VaultName 'Contoso' -Name 'FinanceSecret' -Force -Confirm:$False
```

This command removes the secret named FinanceSecret from the key vault named Contoso.
The command specifies the *Force* and *Confirm* parameters, and, therefore, the cmdlet does not prompt you for confirmation.

## PARAMETERS

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

### -Name
Specifies the name of a secret.
This cmdlet constructs the fully qualified domain name (FQDN) of a secret based on the name that this parameter specifies, the name of the key vault, and your current environment.

```yaml
Type: String
Parameter Sets: (All)
Aliases: SecretName

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -PassThru
Indicates that this cmdlet returns a **Microsoft.Azure.Commands.KeyVault.Models.Secret** object.
By default, this cmdlet does not generate any output.

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

### -VaultName
Specifies the name of the key vault to which the secret belongs.
This cmdlet constructs the FQDN of a key vault based on the name that this parameter specifies and your current environment.

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
The cmdlet is not run.Shows what would happen if the cmdlet runs.
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

### String

## OUTPUTS

### Microsoft.Azure.Commands.KeyVault.Models.Secret
This cmdlet returns a value only if you specify the *PassThru* parameter.

## NOTES

## RELATED LINKS

[Get-AzureKeyVaultSecret](xref:ResourceManager/AzureRM.KeyVault/v2.6.0/Get-AzureKeyVaultSecret.md)

[Set-AzureKeyVaultSecret](xref:ResourceManager/AzureRM.KeyVault/v2.6.0/Set-AzureKeyVaultSecret.md)

