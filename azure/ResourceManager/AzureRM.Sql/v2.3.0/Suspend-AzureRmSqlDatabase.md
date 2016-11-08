---
external help file: Microsoft.Azure.Commands.Sql.dll-Help.xml
ms.assetid: B083D3E9-A931-4793-8B34-3B4FB8D46663
online version: 
schema: 2.0.0
updated_at: 11/8/2016 12:38 AM
ms.date: 11/8/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Sql/v2.3.0/Suspend-AzureRmSqlDatabase.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04b9ae2d1c44a3ada330f570237886794cede893/azureps-cmdlets-docs/ResourceManager/AzureRM.Sql/v2.3.0/Suspend-AzureRmSqlDatabase.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Suspend-AzureRmSqlDatabase

## SYNOPSIS
Suspends a SQL Data Warehouse database.

## SYNTAX

```
Suspend-AzureRmSqlDatabase [-ServerName] <String> -DatabaseName <String> [-ResourceGroupName] <String>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

## DESCRIPTION
The **Suspend-AzureRmSqlDatabase** cmdlet suspends an Azure SQL Data Warehouse database.

## EXAMPLES

### Example 1: Suspends an Azure SQL Data Warehouse database
```
PS C:\>Suspend-AzureRmSqlDatabase -ResourceGroupName "ResourceGroup01" -ServerName "Server01" -DatabaseName "Database01"
```

This command suspends an active Azure SQL Data Warehouse database.

## PARAMETERS

### -ServerName
Specifies the name of the server which hosts the database.

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

### -DatabaseName
Specifies the name of the database that this cmdlet suspends.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of the resource group to which the server is assigned.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
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

### -Confirm
Prompts you for confirmation before running the cmdlet.Prompts you for confirmation before running the cmdlet.

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

### Microsoft.Azure.Commands.Sql.Database.Model.AzureSqlDatabaseModel

## OUTPUTS

### Microsoft.Azure.Commands.Sql.Database.Model.AzureSqlDatabaseModel

## NOTES
* The **Suspend-AzureRmSqlDatabase** cmdlet works only on Azure SQL Data Warehouse databases. This operation is not supported on Azure SQL Database Basic, Standard and Premium editions.

## RELATED LINKS

[Get-AzureRmSqlDatabase](xref:ResourceManager/AzureRM.Sql/v2.3.0/Get-AzureRmSqlDatabase.md)

[New-AzureRmSqlDatabase](xref:ResourceManager/AzureRM.Sql/v2.3.0/New-AzureRmSqlDatabase.md)

[Remove-AzureRmSqlDatabase](xref:ResourceManager/AzureRM.Sql/v2.3.0/Remove-AzureRmSqlDatabase.md)

[Resume-AzureRmSqlDatabase](xref:ResourceManager/AzureRM.Sql/v2.3.0/Resume-AzureRmSqlDatabase.md)

[Set-AzureRmSqlDatabase](xref:ResourceManager/AzureRM.Sql/v2.3.0/Set-AzureRmSqlDatabase.md)

[Azure SQL Database Cmdlets](xref:ResourceManager/AzureRM.Sql/v2.3.0/AzureRM.Sql.md)

