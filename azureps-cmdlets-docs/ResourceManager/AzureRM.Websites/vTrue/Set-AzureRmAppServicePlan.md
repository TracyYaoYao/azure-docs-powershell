---
external help file: Microsoft.Azure.Commands.Websites.dll-Help.xml
ms.assetid: 32D45795-FBCD-4157-BF45-41BD1F61782E
online version: 
schema: 2.0.0
---

# Set-AzureRmAppServicePlan

## SYNOPSIS
Sets an Azure App Service plan.

## SYNTAX

### S1
```
Set-AzureRmAppServicePlan [[-AdminSiteName] <String>] [[-Tier] <String>] [[-NumberofWorkers] <Int32>]
 [[-WorkerSize] <String>] [[-PerSiteScaling] <Boolean>][-ResourceGroupName] <String> [-Name] <String> [<CommonParameters>]
```

### S2
```
Set-AzureRmAppServicePlan [-AppServicePlan] <ServerFarmWithRichSku> [<CommonParameters>]
```

## DESCRIPTION
The **Set-AzureRmAppServicePlan** cmdlet sets an Azure App Service plan.

## EXAMPLES

### 1:
```
PS C:\> Set-AzureRmAppServicePlan -ResourceGroupName "Default-Web-WestUS" -Name "ContosoAppServPlan" -PerSiteScaling  $true
```

This command sets the PerSiteScaling option to true on the App Service plan named ContosoAppServPlan 
    that belongs to the resource group named Default-Web-WestUS.

## PARAMETERS

### -AdminSiteName
Admin Site Name

```yaml
Type: String
Parameter Sets: S1
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Tier
Tier

```yaml
Type: String
Parameter Sets: S1
Aliases: 

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NumberofWorkers
Number Of Workers

```yaml
Type: Int32
Parameter Sets: S1
Aliases: 

Required: False
Position: 4
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WorkerSize
Worker Size

```yaml
Type: String
Parameter Sets: S1
Aliases: 

Required: False
Position: 5
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PerSiteScaling
Per Site Scaling Boolean

```yaml
Type: Boolean
Parameter Sets: S1
Aliases: 

Required: False
Position: 6
Default value: False
Accept pipeline input: False
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

### -Name
Specifies the name of an App service plan.

```yaml
Type: String
Parameter Sets: S1
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AppServicePlan
App Service Plan Object

```yaml
Type: ServerFarmWithRichSku
Parameter Sets: S2
Aliases: 

Required: True
Position: 0
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

[Get-AzureRmWebApp](./Get-AzureRmWebApp.md)

[New-AzureRmWebApp](./New-AzureRmWebApp.md)

[Remove-AzureRmWebApp](./Remove-AzureRmWebApp.md)

[Restart-AzureRmWebApp](./Restart-AzureRmWebApp.md)

[Start-AzureRmWebApp](./Start-AzureRmWebApp.md)

[Stop-AzureRmWebApp](./Stop-AzureRmWebApp.md)

