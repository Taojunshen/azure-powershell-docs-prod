---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.dll-Help.xml
online version: .\Get-AzureDeploymentEvent.md
schema: 2.0.0
ms.assetid: D73A02F6-CDDF-4B21-A841-17117CAB6D40
updated_at: 10/18/2016 9:38 PM
ms.date: 10/18/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v0.9.8/Get-AzureDeployment.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/23cdb8705d4ab9807c0e21b238f3b134a7d49c7d/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v0.9.8/Get-AzureDeployment.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AzureDeployment

## SYNOPSIS
Gets details of a deployment.

## SYNTAX

```
Get-AzureDeployment [-ServiceName] <String> [[-Slot] <String>] [-Profile <AzureProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureDeployment** cmdlet gets details of an Azure deployment.
Specify the name of the Azure service and the slot of the deployment.

## EXAMPLES

### Example 1: Get details for a production deployment
```
PS C:\>Get-AzureDeployment -ServiceName "ContosoService"
```

This command returns the details of the deployment for the service named ContosoService.
This command does not specify a slot.
Therefore, the command uses the default value of Production.

### Example 2: Get details for a staging deployment
```
PS C:\>Get-AzureDeployment -ServiceName "ContosoService" -Slot "Staging"
```

This command returns the details of the staging deployment of ContosoService.

## PARAMETERS

### -ServiceName
Specifies the name of the service.

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

### -Slot
Specifies the environment of the deployment.
Valid values are: Staging or Production.
The default value is Production.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: False
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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureDeploymentEvent](.\Get-AzureDeploymentEvent.md)

[Move-AzureDeployment](.\Move-AzureDeployment.md)

[New-AzureDeployment](.\New-AzureDeployment.md)

[Remove-AzureDeployment](.\Remove-AzureDeployment.md)

[Set-AzureDeployment](.\Set-AzureDeployment.md)

