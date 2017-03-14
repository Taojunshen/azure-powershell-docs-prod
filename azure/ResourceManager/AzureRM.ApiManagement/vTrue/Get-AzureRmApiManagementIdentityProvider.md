---
external help file: Microsoft.Azure.Commands.ApiManagement.ServiceManagement.dll-Help.xml
online version: 
schema: 2.0.0
updated_at: 3/10/2017 7:40 PM
ms.date: 3/10/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ResourceManager/AzureRM.ApiManagement/vTrue/Get-AzureRmApiManagementIdentityProvider.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ResourceManager/AzureRM.ApiManagement/vTrue/Get-AzureRmApiManagementIdentityProvider.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/16665bd43882b185a8143de54e498a0463907aa7/azureps-cmdlets-docs/ResourceManager/AzureRM.ApiManagement/vTrue/Get-AzureRmApiManagementIdentityProvider.md
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

# Get-AzureRmApiManagementIdentityProvider

## SYNOPSIS
Get the identity provider configuration details.

## SYNTAX

### AllIdentityProviders (Default)
```
Get-AzureRmApiManagementIdentityProvider -Context <PsApiManagementContext>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

### IdentityProviderByType
```
Get-AzureRmApiManagementIdentityProvider -Context <PsApiManagementContext>
 -Type <PsApiManagementIdentityProviderType> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

## DESCRIPTION
Get the identity provider configuration details.

## EXAMPLES

### --------------------------  Example 1  --------------------------
@{paragraph=PS C:\\\>}

```
Get-AzureRmApiManagementIdentityProvider -Context $context
```

Get all the identity provider Configuration on the service.

### --------------------------  Example 2  --------------------------
@{paragraph=PS C:\\\>}

```
Get-AzureRmApiManagementIdentityProvider -Context $context -Type Aad
```

Gets the Identity Provider Configuration of Azure Active Directory.

## PARAMETERS

### -Context
Instance of PsApiManagementContext.
This parameter is required.

```yaml
Type: PsApiManagementContext
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
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

### -Type
Identifier of a Identity Provider.
If specified will try to find identity provider configuration by the identifier.
This parameter is optional.

```yaml
Type: PsApiManagementIdentityProviderType
Parameter Sets: IdentityProviderByType
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

### IList<Microsoft.Azure.Commands.ApiManagement.ServiceManagement.Models.PsApiManagementIdentityProvider>

### Microsoft.Azure.Commands.ApiManagement.ServiceManagement.Models.PsApiManagementIdentityProvider

## NOTES

## RELATED LINKS

