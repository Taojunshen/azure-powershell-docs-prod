---
external help file: Microsoft.Azure.Commands.ResourceManager.Automation.dll-Help.xml
ms.assetid: 5C86545A-93DD-4B3C-96B2-FA6ED740448D
online version: 
schema: 2.0.0
updated_at: 11/8/2016 12:38 AM
ms.date: 11/8/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Automation/v2.3.0/Start-AzureRMAutomationRunbook.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04b9ae2d1c44a3ada330f570237886794cede893/azureps-cmdlets-docs/ResourceManager/AzureRM.Automation/v2.3.0/Start-AzureRMAutomationRunbook.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Start-AzureRmAutomationRunbook

## SYNOPSIS
Starts a runbook job.

## SYNTAX

### ByAsynchronousReturnJob (Default)
```
Start-AzureRmAutomationRunbook [-Name] <String> [-Parameters <IDictionary>] [-RunOn <String>]
 [-ResourceGroupName] <String> [-AutomationAccountName] <String> [<CommonParameters>]
```

### BySynchronousReturnJobOutput
```
Start-AzureRmAutomationRunbook [-Name] <String> [-Parameters <IDictionary>] [-RunOn <String>] [-Wait]
 [-MaxWaitSeconds <Int32>] [-ResourceGroupName] <String> [-AutomationAccountName] <String> [<CommonParameters>]
```

## DESCRIPTION
The **Start-AzureRmAutomationRunbook** cmdlet starts an Azure Automation runbook job.
Specify the ID or name of a runbook.

## EXAMPLES

### Example 1: Start a runbook job
```
PS C:\>Start-AzureRmAutomationRunbook -AutomationAccountName "Contoso17" -Name "Runbk01" -ResourceGroupName "ResourceGroup01"
```

This command starts a runbook job for the runbook named Runbk01 in the Azure Automation account named Contoso17.

## PARAMETERS

### -AutomationAccountName
```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Name
```yaml
Type: String
Parameter Sets: (All)
Aliases: RunbookName

Required: True
Position: 3
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Parameters
```yaml
Type: IDictionary
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResourceGroupName
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

### -RunOn
```yaml
Type: String
Parameter Sets: (All)
Aliases: HybridWorker

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Wait
```yaml
Type: SwitchParameter
Parameter Sets: BySynchronousReturnJobOutput
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MaxWaitSeconds
```yaml
Type: Int32
Parameter Sets: BySynchronousReturnJobOutput
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

## OUTPUTS

### Microsoft.Azure.Commands.Automation.Model.Job

## NOTES

## RELATED LINKS

[Export-AzureRmAutomationRunbook](xref:ResourceManager/AzureRM.Automation/v2.3.0/Export-AzureRMAutomationRunbook.md)

[Get-AzureRmAutomationRunbook](xref:ResourceManager/AzureRM.Automation/v2.3.0/Get-AzureRMAutomationRunbook.md)

[Import-AzureRmAutomationRunbook](xref:ResourceManager/AzureRM.Automation/v2.3.0/Import-AzureRMAutomationRunbook.md)

[New-AzureRmAutomationRunbook](xref:ResourceManager/AzureRM.Automation/v2.3.0/New-AzureRMAutomationRunbook.md)

[New-AzureRmAutomationRunbook](xref:ResourceManager/AzureRM.Automation/v2.3.0/New-AzureRMAutomationRunbook.md)

[Publish-AzureRmAutomationRunbook](xref:ResourceManager/AzureRM.Automation/v2.3.0/Publish-AzureRMAutomationRunbook.md)

[Remove-AzureRmAutomationRunbook](xref:ResourceManager/AzureRM.Automation/v2.3.0/Remove-AzureRMAutomationRunbook.md)

[Set-AzureRmAutomationRunbook](xref:ResourceManager/AzureRM.Automation/v2.3.0/Set-AzureRMAutomationRunbook.md)

