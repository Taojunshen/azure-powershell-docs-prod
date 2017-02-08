---
external help file: Microsoft.RightsManagementServices.Online.Admin.PowerShell.dll-Help.xml
online version: http://go.microsoft.com/fwlink/?LinkID=400629
schema: 2.0.0
ms.assetid: BE20B1AF-4D47-4182-A46A-2FB0AB504A93
updated_at: 2/4/2017 5:39 PM
ms.date: 2/4/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/master/Azure%20Information%20Protection/AADRM/vlatest/New-AadrmRightsDefinition.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/master/Azure%20Information%20Protection/AADRM/vlatest/New-AadrmRightsDefinition.md
gitcommit: https://github.com/Azure/azure-docs-powershell-aip/blob/6ffafc7c33a2088f5b1357f508b53e2bb981e987/Azure%20Information%20Protection/AADRM/vlatest/New-AadrmRightsDefinition.md
ms.topic: reference
ms.prod: powershell
ms.technology: Azure Powershell
author: cabailey
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: cabailey
open_to_public_contributors: False
ms.service: rights-management
---

# New-AadrmRightsDefinition

## SYNOPSIS
Creates a Rights Definition object for Rights Management.

## SYNTAX

```
New-AadrmRightsDefinition -EmailAddress <String> -Rights <System.Collections.Generic.List`1[System.String]>
 [<CommonParameters>]
```

## DESCRIPTION
The **New-AadrmRightsDefinition** cmdlet creates a **Rights Definition** object that you store as a variable and then use to create or update a custom rights policy template when you use the [Add-AadrmTemplate](./Add-AadrmTemplate.md) or [Set-AadrmTemplateProperty](./Set-AadrmTemplateProperty.md) cmdlet.

A **Rights Definition** object expresses the rights of a user or group to content that Azure Rights Management protects.

## EXAMPLES

### Example 1: Create a rights definition object for a user
```
PS C:\>$R1 = New-AadrmRightsDefinition -EmailAddress "ElisaDaugherty@Contoso.com" -Rights "VIEW","DOCEDIT"
```

This command creates a rights definition object for the specified user and stores this policy in a variable named R1, which can then be used to create or update a custom template. 

The command includes the rights VIEW and DOCEDIT for a user in the Contoso organization.

### Example 2: Create a rights definition object for all users
```
PS C:\>$R2 = New-AadrmRightsDefinition -EmailAddress "AllStaff-7184AB3F-CCD1-46F3-8233-3E09E9CF0E66@contoso.onmicrosoft.com" -Rights "VIEW"
```

This command creates a rights definition object for all users in the organization and stores this policy in a variable named R2, which can then be used to create or update a custom template.

The command includes the VIEW right for all users in the Contoso organization, by using the automatically created "AllStaff-7184AB3F-CCD1-46F3-8233-3E09E9CF0E66@{tenant_name}.onmicrosoft.com" group that is created for the organization when the Azure Rights Management service is activated.

## PARAMETERS

### -EmailAddress
Specifies the email address of a user or group. You can specify external email addresses for users outside your organization but external email addresses for groups are not currently supported.

The cmdlet associates the rights that the *Rights* parameter specifies to the user or group that the address specifies.

Tip: If you want to specify all users in your organization, use the automatically created group, AllStaff-7184AB3F-CCD1-46F3-8233-3E09E9CF0E66@{tenant_name}.onmicrosoft.com. For example, this group might look like the following for Contoso: **AllStaff-7184AB3F-CCD1-46F3-8233-3E09E9CF0E66@contoso.onmicrosoft.com**. You can see your organization's automatically created email address if you copy one of the default rights policy templates in the Azure portal, and then identify the USER NAME on the RIGHTS page.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Rights
Specifies a list of rights. The list contains one or more of the following:

- **VIEW**: Interpreted by most applications as allowed to present the data on the screen.

- **EDIT**: Interpreted by most applications as allowed to modify content in the document and save it.

- **DOCEDIT**: Interpreted by most applications as allowed to modify the content of the document.

- **EXTRACT**: Interpreted by most applications as allowed to copy the content to the clipboard or otherwise extract the content in unencrypted form.

- **OBJMODEL**: Interpreted by most applications as allowed to access the document programmatically; for example, by using macros.

- **EXPORT**: Interpreted by most applications as allowed to save the file in unencrypted form. For example, this right allows you to save in a different file format that does not support protection.

- **PRINT**: Interpreted by most applications as allowed to print the document.

- **OWNER**: User has all rights on the document, including the ability to remove protection.

- **FORWARD**: Interpreted by most applications as allowed to forward an email message, and to add recipients to the To and Cc lines.

- **REPLY**: Interpreted by most applications as allowed to select reply to an email message, without allowing changes in the To or Cc lines.

- **REPLYALL**: Interpreted by most applications as allowed to reply to all recipients of an email message, but does not allow the user to add recipients to the To or Cc lines.

Note: For clarity, the documentation and display text from the module shows these rights as all upper-case letters. However, the values are not case-sensitive and you can specify them in lower or upper case.

For more information about the usage rights, see Configuring usage rights for [Azure Rights Management](https://docs.microsoft.com/rights-management/deploy-use/configure-usage-rights) (https://docs.microsoft.com/rights-management/deploy-use/configure-usage-rights) on the Microsoft documentation site.

```yaml
Type: System.Collections.Generic.List`1[System.String]
Parameter Sets: (All)
Aliases:

Required: True
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

[Add-AadrmTemplate](xref:AADRM/vlatest/Add-AadrmTemplate.md)

[Set-AadrmTemplateProperty](xref:AADRM/vlatest/Set-AadrmTemplateProperty.md)

[Azure Rights Management](https://docs.microsoft.com/rights-management/deploy-use/configure-usage-rights)
