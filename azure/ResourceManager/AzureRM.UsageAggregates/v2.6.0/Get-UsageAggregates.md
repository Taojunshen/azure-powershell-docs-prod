---
external help file: Microsoft.Azure.Commands.UsageAggregates.dll-Help.xml
ms.assetid: 52B3ECCB-80E5-4E16-954A-B83D0BDC7E22
online version: 
schema: 2.0.0
updated_at: 3/11/2017 3:58 PM
ms.date: 3/11/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.UsageAggregates/v2.6.0/Get-UsageAggregates.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.UsageAggregates/v2.6.0/Get-UsageAggregates.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/bc71000aa3c7f754b95442dcc415a7324626a15c/azureps-cmdlets-docs/ResourceManager/AzureRM.UsageAggregates/v2.6.0/Get-UsageAggregates.md
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

# Get-UsageAggregates

## SYNOPSIS
Gets the reported Azure subscription usage details.

## SYNTAX

```
Get-UsageAggregates -ReportedStartTime <DateTime> -ReportedEndTime <DateTime>
 [-AggregationGranularity <AggregationGranularity>] [-ShowDetails <Boolean>] [-ContinuationToken <String>]
 [<CommonParameters>]
```

## DESCRIPTION
The **Get-UsageAggregates** cmdlet gets aggregated Azure subscription usage data by the following properties: 

- Start and end times of when the usage was reported.

- Aggregation precision, either daily or hourly.

- Instance level detail for multiple instances of the same resource.

For consistent results, the returned data is based on when the usage details were reported by the Azure resource.

For more information, see Azure Billing REST API Referencehttps://msdn.microsoft.com/library/azure/1ea5b323-54bb-423d-916f-190de96c6a3c (https://msdn.microsoft.com/library/azure/1ea5b323-54bb-423d-916f-190de96c6a3c) in the Microsoft Developer Network library.

## EXAMPLES

### Example 1: Retrieve subscription data
```
PS C:\>Get-UsageAggregates -ReportedStartTime "5/2/2015" -ReportedEndTime "5/5/2015"
```

This command retrieves the reported usage data for the subscription between 5/2/2015 and 5/5/2015.

## PARAMETERS

### -AggregationGranularity
Specifies the aggregation precision of the data.
Valid values are: Daily and Hourly.

The default value is Daily.

```yaml
Type: AggregationGranularity
Parameter Sets: (All)
Aliases: 
Accepted values: Daily, Hourly

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ContinuationToken
Specifies the continuation token that was retrieved from the response body in the previous call.
For a large result set, responses are paged by using continuation tokens.
The continuation token serves as a bookmark for progress.
If you do not specify this parameter, the data is retrieved from the beginning of the day or hour specified in *ReportedStartTime*.
We recommend that you follow the next link in the response to page though the data.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ReportedEndTime
Specifies the reported end time for when resource usage was recorded in the Azure billing system.

Azure is a distributed system, spanning multiple datacenters around the world, so there is a delay between when the resource was actually consumed, which is the resource usage time, and when the usage event reached the billing system, which is the resource usage reported time.
In order to get all usage events for a subscription that are reported for a time period, you query by reported time.
Even though you query by reported time, the cmdlet aggregates the response data by the resource usage time.
The resource usage data is the useful pivot for analyzing the data.

```yaml
Type: DateTime
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ReportedStartTime
Specifies the reported start time for when resource usage was recorded in the Azure billing system.

```yaml
Type: DateTime
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ShowDetails
Indicates whether this cmdlet returns instance-level details with the usage data.

The default value is $True.

If $False, the service aggregates the results on the server side, and therefore returns fewer aggregate groups.
For example, if you are running three websites, by default you will get three line items for website consumption.
However, when the value is $False, all the data for the same **subscriptionId**, **meterId**, **usageStartTime**, and **usageEndTime** is collapsed into a single line item.

```yaml
Type: Boolean
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

## OUTPUTS

## NOTES

## RELATED LINKS
