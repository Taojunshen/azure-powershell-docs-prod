---
external help file: Microsoft.Azure.Commands.AzureBackup.dll-Help.xml
ms.assetid: C5126E20-0A93-4ACE-8297-F1E8E17BEF53
online version: 
schema: 2.0.0
updated_at: 3/4/2017 12:37 AM
ms.date: 3/4/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ResourceManager/AzureRM.Backup/vTrue/Wait-AzureRmBackupJob.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ResourceManager/AzureRM.Backup/vTrue/Wait-AzureRmBackupJob.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/91cff23a000b99dc60ec82204d789c7ace1d7134/azureps-cmdlets-docs/ResourceManager/AzureRM.Backup/vTrue/Wait-AzureRmBackupJob.md
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

# Wait-AzureRmBackupJob

## SYNOPSIS
Waits for a Backup job to finish.

## SYNTAX

```
Wait-AzureRmBackupJob -Job <Object> [-TimeOut <Int64>] [<CommonParameters>]
```

## DESCRIPTION
The **Wait-AzureRmBackupJob** cmdlet waits for an Azure Backup job to finish.
Backup jobs can take a long time.
If you run a backup job as part of a script, you may want to force the script to wait for job to finish before it continues to other tasks.

A script that includes this cmdlet can be simpler than one that polls the Backup service for the job status.

## EXAMPLES

### 1:
```

```

## PARAMETERS

### -Job
Specifies a job that this cmdlet cancels.
To obtain an **AzureRmBackupJob** object, use the Get-AzureRmBackupJob cmdlet.

```yaml
Type: Object
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -TimeOut
Specifies the maximum time, in seconds, that this cmdlet waits for the job to finish.
We recommend that you specify a time-out value.

```yaml
Type: Int64
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

### AzureRmBackupJob

## OUTPUTS

### AzureRmBackupJob[]

## NOTES

## RELATED LINKS

[Get-AzureRmBackupJob](xref:ResourceManager/AzureRM.Backup/vTrue/Get-AzureRmBackupJob.md)

[Stop-AzureRmBackupJob](xref:ResourceManager/AzureRM.Backup/vTrue/Stop-AzureRmBackupJob.md)

