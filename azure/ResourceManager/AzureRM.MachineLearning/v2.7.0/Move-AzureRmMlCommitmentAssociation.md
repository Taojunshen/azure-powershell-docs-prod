---
external help file: Microsoft.Azure.Commands.MachineLearning.dll-Help.xml
online version: 
schema: 2.0.0
updated_at: 3/11/2017 2:20 AM
ms.date: 3/11/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.MachineLearning/v2.7.0/Move-AzureRmMlCommitmentAssociation.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.MachineLearning/v2.7.0/Move-AzureRmMlCommitmentAssociation.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04f63f6e685743ace2c57eb157574e34e8610b1c/azureps-cmdlets-docs/ResourceManager/AzureRM.MachineLearning/v2.7.0/Move-AzureRmMlCommitmentAssociation.md
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

# Move-AzureRmMlCommitmentAssociation

## SYNOPSIS
Moves a commitment association from one commitment plan to another.

## SYNTAX

```
Move-AzureRmMlCommitmentAssociation -ResourceGroupName <String> -CommitmentPlanName <String> -Name <String>
 -DestinationPlanId <String> [-Confirm]
```

## DESCRIPTION
Moves a commitment association resource from its parent commitment plan to another commitment plan.

## EXAMPLES

### --------------------------  Example 1: Move a commitment association  --------------------------
@{paragraph=PS C:\\\>}

```
Get-AzureRmMlCommitmentAssociation -ResourceGroupName "MyResourceGroup" -CommitmentPlanName "SourceCommitmentPlanName" -Name "MyCommitmentAssociationName" -DestinationPlanId "/subscriptions/MySubscriptionId/resourceGroups/MyResourceGroup/providers/Microsoft.MachineLearning/commitmentPlans/DestinationCommitmentPlanName"
```

## PARAMETERS

### -CommitmentPlanName
The name of the Azure ML commitment plan.

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

### -DestinationPlanId
The Azure resource ID of the destination Azure ML commitment plan.

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

### -Name
The name of the Azure ML commitment association.

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

### -ResourceGroupName
The name of the resource group for the Azure ML commitment association.

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

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

### Microsoft.Azure.Management.MachineLearning.CommitmentPlans.Models.CommitmentPlan
Microsoft.Azure.Management.MachineLearning.CommitmentPlans.Models.CommitmentPlan[]

## NOTES
Keywords: azure, azurerm, arm, resource, management, manager, machine, machine learning, azureml

## RELATED LINKS

