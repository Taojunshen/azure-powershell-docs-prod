---
external help file: Microsoft.WindowsAzure.Commands.SqlDatabase.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: FEA2AB4E-1750-4E5A-B0EA-24532215B23A
updated_at: 11/11/2016 11:03 PM
ms.date: 11/11/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.SQLDatabase/v1.6.1/Get-AzureSqlRecoverableDatabase.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.SQLDatabase/v1.6.1/Get-AzureSqlRecoverableDatabase.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/79eeb985ea480979357fb4695832a0c3d29a48bf/azureps-cmdlets-docs/ServiceManagement/Azure.SQLDatabase/v1.6.1/Get-AzureSqlRecoverableDatabase.md
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

# Get-AzureSqlRecoverableDatabase

## SYNOPSIS
Gets recoverable databases from a specified server.

## SYNTAX

### AllDatabasesOnGivenServer (Default)
```
Get-AzureSqlRecoverableDatabase -ServerName <String> [-Profile <AzureSMProfile>] [<CommonParameters>]
```

### GivenDatabaseOnGivenServer
```
Get-AzureSqlRecoverableDatabase -ServerName <String> -DatabaseName <String> [-Profile <AzureSMProfile>]
 [<CommonParameters>]
```

### GivenDatabaseObject
```
Get-AzureSqlRecoverableDatabase -Database <RecoverableDatabase> [-Profile <AzureSMProfile>]
 [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureSqlRecoverableDatabase** cmdlet gets recoverable databases from a specified server.
This cmdlet gets a specific recoverable database or all recoverable databases on a server.

## EXAMPLES

### Example 1: Get all recoverable databases
```
PS C:\>Get-AzureSqlRecoverableDatabase -ServerName "server1"
```

This command gets all recoverable databases on the server named Server01.

### Example 2: Get a specific recoverable database
```
PS C:\>Get-AzureSqlRecoverableDatabase -ServerName "Server01" -DatabaseName "Database17"
```

This command gets retrieves the database named Database17 on the server named Server01.

## PARAMETERS

### -ServerName
Specifies the name of the server from which this cmdlet gets recoverable databases.

```yaml
Type: String
Parameter Sets: AllDatabasesOnGivenServer, GivenDatabaseOnGivenServer
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DatabaseName
Specifies the name of the recoverable database that this cmdlet gets.

```yaml
Type: String
Parameter Sets: GivenDatabaseOnGivenServer
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Database
Specifies an object that represents the recoverable database that this cmdlet gets.

```yaml
Type: RecoverableDatabase
Parameter Sets: GivenDatabaseObject
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Profile
ps_azureprofile_description

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

### Microsoft.WindowsAzure.Management.Sql.Models.RecoverableDatabase

## OUTPUTS

### IEnumerable<Microsoft.WindowsAzure.Management.Sql.Models.RecoverableDatabase>

## NOTES
* You must use certificate-based authentication to run this cmdlet. Run the following commands on the computer where run this cmdlet: 

`PS C:\\\> $subId = \<Subscription ID\>`
`PS C:\\\> $thumbprint = \<Certificate Thumbprint\>`
`PS C:\\\> $myCert = Get-Item Cert:\CurrentUser\My\$thumbprint`
`PS C:\\\> Set-AzureSubscription -SubscriptionName "mySubscription" -SubscriptionId $subId -Certificate $myCert`
`PS C:\\\> Select-AzureSubscription -SubscriptionName "mySubscription"`

## RELATED LINKS

[Azure SQL Database](https://azure.microsoft.com/en-us/services/sql-database/)

[Get Recoverable Database](https://msdn.microsoft.com/en-us/library/azure/dn800985.aspx)

[Operations for Azure SQL Databases](https://msdn.microsoft.com/en-us/library/azure/dn505719.aspx)

[Start-AzureSqlDatabaseRecovery](xref:ServiceManagement/Azure.SQLDatabase/v1.6.1/Start-AzureSqlDatabaseRecovery.md)


