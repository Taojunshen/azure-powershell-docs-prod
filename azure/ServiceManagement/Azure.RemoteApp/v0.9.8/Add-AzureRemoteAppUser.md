---
external help file: Microsoft.WindowsAzure.Commands.RemoteApp.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: DF927EC1-AA02-4BEA-A617-3FE0B59B88D7
updated_at: 11/1/2016 10:24 PM
ms.date: 11/1/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.RemoteApp/v0.9.8/Add-AzureRemoteAppUser.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.RemoteApp/v0.9.8/Add-AzureRemoteAppUser.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/f59f3ef60bc592383812213e69fd77ba950759ed/azureps-cmdlets-docs/ServiceManagement/Azure.RemoteApp/v0.9.8/Add-AzureRemoteAppUser.md
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

# Add-AzureRemoteAppUser

## SYNOPSIS
Adds a user to a RemoteApp collection.

## SYNTAX

```
Add-AzureRemoteAppUser [-CollectionName] <String> [-Type] <PrincipalProviderType> [-UserUpn] <String[]>
 [-Profile <AzureProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Add-AzureRemoteAppUser** cmdlet adds a user to an Azure RemoteApp collection.

## EXAMPLES

### Example 1: Add a user using a Microsoft Account
```
PS C:\>Add-AzureRemoteAppUser -CollectionName "Contoso" -UserType MicrosoftAccount -UserUpn "PattiFuller@contoso.com"
```

This command adds the Microsoft Account PattiFuller@contoso.com to the collection named Contoso.

### 1: Add a user using an Azure Active Directory account
```
PS C:\>Add-AzureRemoteAppUser -CollectionName "Contoso" -UserType OrgId -UserUpn "PattiFuller@contoso.com"
```

This command adds the Azure Active Directory account PattiFuller@contoso.com to the collection named Contoso.

## PARAMETERS

### -CollectionName
Specifies the name of the RemoteApp collection.

```yaml
Type: String
Parameter Sets: (All)
Aliases: Name

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Profile
Specifies the Azure profile from which this cmdlet reads.
If you do not specify a profile, this cmdlet reads from the local default profile.

```yaml
Type: AzureProfile
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Type
Specifies a user type.
The acceptable values for this parameter are: OrgId or MicrosoftAccount.

```yaml
Type: PrincipalProviderType
Parameter Sets: (All)
Aliases: 
Accepted values: OrgId, MicrosoftAccount

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -UserUpn
Specifies the User Principal Name (UPN) of a user, for example, PattiFuller@contoso.com.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
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

[Get-AzureRemoteAppUser](xref:ServiceManagement/Azure.RemoteApp/v0.9.8/Get-AzureRemoteAppUser.md)

[Remove-AzureRemoteAppUser](xref:ServiceManagement/Azure.RemoteApp/v0.9.8/Remove-AzureRemoteAppUser.md)


