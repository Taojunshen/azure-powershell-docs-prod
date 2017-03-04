---
external help file: Microsoft.Azure.Commands.Resources.dll-Help.xml
ms.assetid: C61FA834-BEBE-4DBF-888F-C6CB8CC95390
online version:
schema: 2.0.0
updated_at: 3/4/2017 6:58 PM
ms.date: 3/4/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v3.3.0/Remove-AzureRmADAppCredential.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v3.3.0/Remove-AzureRmADAppCredential.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/aa2ae758d5790a27662a17dfad5119b5b8987494/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v3.3.0/Remove-AzureRmADAppCredential.md
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

# Remove-AzureRmADAppCredential

## SYNOPSIS
Removes a credential from an application.

## SYNTAX

### ApplicationObjectIdWithKeyIdParameterSet (Default)
```
Remove-AzureRmADAppCredential -ObjectId <String> -KeyId <Guid> [-Force] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [-WhatIf] [-Confirm]
```

### ApplicationObjectIdWithAllParameterSet
```
Remove-AzureRmADAppCredential -ObjectId <String> [-All] [-Force] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [-WhatIf] [-Confirm]
```

### ApplicationIdWithAllParameterSet
```
Remove-AzureRmADAppCredential -ApplicationId <String> [-All] [-Force] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [-WhatIf] [-Confirm]
```

### ApplicationIdWithKeyIdParameterSet
```
Remove-AzureRmADAppCredential -ApplicationId <String> -KeyId <Guid> [-Force]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [-WhatIf] [-Confirm]
```

## DESCRIPTION
The **Remove-AzureRmADAppCredential** cmdlet can be used to remove a credential key from an application in the case of a compromise or as part of credential key rollover expiration.
The application is identified by supplying either the object ID or AppId.
The credential to be removed is identified by its key ID if an individual credential is to be removed or with an 'All' switch to delete all credentials associated with the application.

## EXAMPLES

### Example 1: Remove a credential key from an application

```
PS C:\> Remove-AzureRmADAppCredential -ObjectId 7663d3fb-6f86-4352-9e6d-cf9d50d5ee82 -KeyId 9044423a-60a3-45ac-9ab1-09534157ebb
```

This command removes a credential key from an application.
In this example, the key with Id 9044423a-60a3-45ac-9ab1-09534157ebb will be removed from the application.

### Example 2: Remove a credential key from an application using the application ID


```
PS C:\> Remove-AzureRmADAppCredential -ApplicationId 4589cd6b-3d79-4bb4-93b8-a0b99f3bfc58 -All
```

This command removes a credential key from an application.
In this example, all credentials will be removed from the application associated with the ApplicationId 4589cd6b-3d79-4bb4-93b8-a0b99f3bfc58.

## PARAMETERS

### -ObjectId
Specifies the object ID of the application to remove the credentials from.

```yaml
Type: String
Parameter Sets: ApplicationObjectIdWithKeyIdParameterSet, ApplicationObjectIdWithAllParameterSet
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -KeyId
Specifies the credential key to be removed.
The key Ids for the application can be obtained using the [Get-AzureRmADAppCredential](./Get-AzureRmADAppCredential.md) cmdlet.

```yaml
Type: Guid
Parameter Sets: ApplicationObjectIdWithKeyIdParameterSet, ApplicationIdWithKeyIdParameterSet
Aliases:

Required: True
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
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -All
Indicates that this cmdlet removes all the credentials associated with the application.

```yaml
Type: SwitchParameter
Parameter Sets: ApplicationObjectIdWithAllParameterSet, ApplicationIdWithAllParameterSet
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ApplicationId
Specifies the ID of the application to remove the credentials from.

```yaml
Type: String
Parameter Sets: ApplicationIdWithAllParameterSet, ApplicationIdWithKeyIdParameterSet
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureRmADAppCredential](xref:ResourceManager/AzureRM.Resources/v3.3.0/Get-AzureRmADAppCredential.md)

[New-AzureRmADAppCredential](xref:ResourceManager/AzureRM.Resources/v3.3.0/New-AzureRmADAppCredential.md)

[Get-AzureRmADApplication](xref:ResourceManager/AzureRM.Resources/v3.3.0/Get-AzureRmADApplication.md)
