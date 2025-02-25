---
external help file: 
Module Name: Az.App
online version: https://learn.microsoft.com/powershell/module/az.app/get-azcontainerappsecret
schema: 2.0.0
content_git_url: https://github.com/Azure/azure-powershell/blob/main/src/App/help/Get-AzContainerAppSecret.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/main/src/App/help/Get-AzContainerAppSecret.md
---

# Get-AzContainerAppSecret

## SYNOPSIS
List secrets for a container app

## SYNTAX

```
Get-AzContainerAppSecret -ContainerAppName <String> -ResourceGroupName <String> [-SubscriptionId <String[]>]
 [-DefaultProfile <PSObject>] [-Confirm] [-WhatIf] [<CommonParameters>]
```

## DESCRIPTION
List secrets for a container app

## EXAMPLES

### Example 1: List secrets for a container app
```powershell
Get-AzContainerAppSecret -ContainerAppName azps-containerapp -ResourceGroupName azpstest_gp
```

```output
Name Value
---- -----
key1 value1
```

List secrets for a container app

## PARAMETERS

### -ContainerAppName
Name of the Container App.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DefaultProfile
The credentials, account, tenant, and subscription used for communication with Azure.

```yaml
Type: System.Management.Automation.PSObject
Parameter Sets: (All)
Aliases: AzureRMContext, AzureCredential

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResourceGroupName
The name of the resource group.
The name is case insensitive.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SubscriptionId
The ID of the target subscription.

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: (Get-AzContext).Subscription.Id
Accept pipeline input: False
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### Microsoft.Azure.PowerShell.Cmdlets.App.Models.Api20220301.IContainerAppSecret

## NOTES

ALIASES

## RELATED LINKS

