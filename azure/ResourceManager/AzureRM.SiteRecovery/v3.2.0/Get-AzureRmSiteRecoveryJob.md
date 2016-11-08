---
external help file: Microsoft.Azure.Commands.SiteRecovery.dll-Help.xml
ms.assetid: 874C0981-749B-4161-9AC2-AC445A72EBEB
online version: 
schema: 2.0.0
updated_at: 11/8/2016 12:38 AM
ms.date: 11/8/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.SiteRecovery/v3.2.0/Get-AzureRmSiteRecoveryJob.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04b9ae2d1c44a3ada330f570237886794cede893/azureps-cmdlets-docs/ResourceManager/AzureRM.SiteRecovery/v3.2.0/Get-AzureRmSiteRecoveryJob.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AzureRmSiteRecoveryJob

## SYNOPSIS
Gets the operation information for the current Site Recovery vault.

## SYNTAX

### ByParam (Default)
```
Get-AzureRmSiteRecoveryJob [-StartTime <DateTime>] [-EndTime <DateTime>] [-TargetObjectId <String>]
 [-State <String>] [<CommonParameters>]
```

### ByName
```
Get-AzureRmSiteRecoveryJob -Name <String> [<CommonParameters>]
```

### ByObject
```
Get-AzureRmSiteRecoveryJob -Job <ASRJob> [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmSiteRecoveryJob** cmdlet gets Azure Site Recovery jobs.
You can use this cmdlet to view the operation information for the current Site Recovery vault.

## EXAMPLES

## PARAMETERS

### -StartTime
Specifies the start time for the jobs.
This cmdlet gets all jobs that started after the specified time.

```yaml
Type: DateTime
Parameter Sets: ByParam
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EndTime
Specifies the end time for the jobs.
This cmdlet gets all jobs that started before the specified time.
To obtain a **DateTime** object for this parameter, use the Get-Date cmdlet.
For more information, type `Get-Help Get-Date`.

```yaml
Type: DateTime
Parameter Sets: ByParam
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TargetObjectId
Specifies the ID of the object targeted by the job.

```yaml
Type: String
Parameter Sets: ByParam
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -State
Specifies the input state for a Site Recovery job.
This cmdlet gets all jobs that match the specified state.
The acceptable values for this parameter are:

- NotStarted
- InProgress
- Succeeded
- Other
- Failed
- Cancelled
- Suspended

```yaml
Type: String
Parameter Sets: ByParam
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
Specifies a unique name that identifies the job.

```yaml
Type: String
Parameter Sets: ByName
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Job
Specifies the Site Recovery job.

```yaml
Type: ASRJob
Parameter Sets: ByObject
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Restart-AzureRmSiteRecoveryJob](xref:ResourceManager/AzureRM.SiteRecovery/v3.2.0/Restart-AzureRmSiteRecoveryJob.md)

[Resume-AzureRmSiteRecoveryJob](xref:ResourceManager/AzureRM.SiteRecovery/v3.2.0/Resume-AzureRmSiteRecoveryJob.md)

[Stop-AzureRmSiteRecoveryJob](xref:ResourceManager/AzureRM.SiteRecovery/v3.2.0/Stop-AzureRmSiteRecoveryJob.md)