---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.Network.dll-Help.xml
ms.assetid: D2CE5D4B-8F1F-41FF-9E65-8956FEDD35AE
online version: 
schema: 2.0.0
updated_at: 1/20/2017 9:17 PM
ms.date: 1/20/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Networking/v3.4.0/Get-AzureApplicationGatewaySslCertificate.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Networking/v3.4.0/Get-AzureApplicationGatewaySslCertificate.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/cb06bb906911a2a2e1f57adbafe0c0c97a0b205b/azureps-cmdlets-docs/ServiceManagement/Azure.Networking/v3.4.0/Get-AzureApplicationGatewaySslCertificate.md
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

# Get-AzureApplicationGatewaySslCertificate

## SYNOPSIS
Gets Application Gateway certificates.

## SYNTAX

```
Get-AzureApplicationGatewaySslCertificate -Name <String> [-CertificateName <String>]
 [-Profile <AzureSMProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureApplicationGatewaySslCertificate** cmdlet gets Secure Sockets Layer (SSL) certificates for an Azure Application Gateway.

## EXAMPLES

### Example 1: Get an SSL certificate
```
PS C:\> Get-AzureApplicationGatewaySslCertificate -Name "ApplicationGateway08" -CertificateName "SslCertificate13"
```

This command gets an SSL certificate named SslCertificate13 on the Application Gateway named ApplicationGateway08.

### Example 2: Get all SSL certificates
```
PS C:\> Get-AzureApplicationGatewaySslCertificate -Name "ApplicationGateway08"
```

This command gets all the SSL certificates on the Application Gateway named ApplicationGateway08.

## PARAMETERS

### -CertificateName
Specifies the name of an SSL certificate.
This cmdlet gets the certificate that this parameter specifies.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Name
Specifies the name of the Application Gateway from which this cmdlet gets an SSL certificate.

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

### -Profile
Specifies the Azure profile from which this cmdlet reads.
If you do not specify a profile, this cmdlet reads from the local default profile.

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

### System.String

## OUTPUTS

### Microsoft.Azure.Networking.ApplicationGatewayObjectModel.ApplicationGatewayCertificate, List<Microsoft.Azure.Networking.ApplicationGatewayObjectModel.ApplicationGatewayCertificate>

## NOTES

## RELATED LINKS

[Add-AzureApplicationGatewaySslCertificate](xref:ServiceManagement/Azure.Networking/v3.4.0/Add-AzureApplicationGatewaySslCertificate.md)

[Remove-AzureApplicationGatewaySslCertificate](xref:ServiceManagement/Azure.Networking/v3.4.0/Remove-AzureApplicationGatewaySslCertificate.md)
