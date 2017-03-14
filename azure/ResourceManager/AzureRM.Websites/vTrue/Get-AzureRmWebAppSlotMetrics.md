---
external help file: Microsoft.Azure.Commands.Websites.dll-Help.xml
ms.assetid: 3BCEADF3-15DC-4033-A94A-4C8B4F5E7340
online version: 
schema: 2.0.0
updated_at: 3/13/2017 7:40 PM
ms.date: 3/13/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Websites/vTrue/Get-AzureRmWebAppSlotMetrics.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Websites/vTrue/Get-AzureRmWebAppSlotMetrics.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/7201955e7e0fd9d41b0a087f20717a385bb2fb89/azureps-cmdlets-docs/ResourceManager/AzureRM.Websites/vTrue/Get-AzureRmWebAppSlotMetrics.md
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

# Get-AzureRmWebAppSlotMetrics

## SYNOPSIS
Gets metrics for an Azure Web App slot.

## SYNTAX

### S1
```
Get-AzureRmWebAppSlotMetrics [-Metrics] <String[]> [-StartTime] <DateTime> [[-EndTime] <DateTime>]
 [-Granularity] <String> [-InstanceDetails] [-ResourceGroupName] <String> [-Name] <String> [-Slot] <String>
```

### S2
```
Get-AzureRmWebAppSlotMetrics [-Metrics] <String[]> [-StartTime] <DateTime> [[-EndTime] <DateTime>]
 [-Granularity] <String> [-InstanceDetails] [-WebApp] <Site>
```

## DESCRIPTION
The **Get-AzureRmWebAppSlotMetrics** gets Web App metrics for the specified slot.

## EXAMPLES

### Example 1
```
PS C:\> Get-AzureRmAppServicePlanMetrics -ResourceGroupName "Default-Web-WestUS" -Name "ContosoWebApp" -StartTime 2016-11-30T22:00:00Z -EndTime 2016-11-30T22:30:00Z -Granularity PT1M -Metrics ["Requests"]
```

This command gets Request of the specified Web App per minute(PT1M - Poll Time 1 minute) between StartTime and EndTime

## PARAMETERS

### -EndTime
Specifies the end time in UTC.

```yaml
Type: DateTime
Parameter Sets: (All)
Aliases: 

Required: False
Position: 5
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Granularity
Specifies the granularity of the Web App slot metrics.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 6
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InstanceDetails
Indicates that the cmdlet gets instance details.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: 6
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Metrics
Specifies an array of metrics that this cmdlet gets.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: True
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
Specifies the name of the Web App.

```yaml
Type: String
Parameter Sets: S1
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of the resource group.

```yaml
Type: String
Parameter Sets: S1
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Slot
Specifies the name of the WebApp slot.

```yaml
Type: String
Parameter Sets: S1
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -StartTime
Specifies the start time in UTC.

```yaml
Type: DateTime
Parameter Sets: (All)
Aliases: 

Required: True
Position: 4
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WebApp
Specifies a Web App object.

```yaml
Type: Site
Parameter Sets: S2
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureRMAppServicePlanMetrics](xref:ResourceManager/AzureRM.Websites/vTrue/Get-AzureRmAppServicePlanMetrics.md)

[Get-AzureRmWebApp](xref:ResourceManager/AzureRM.Websites/vTrue/Get-AzureRmWebApp.md)

[Get-AzureRMWebAppSlot](xref:ResourceManager/AzureRM.Websites/vTrue/Get-AzureRMWebAppSlot.md)
