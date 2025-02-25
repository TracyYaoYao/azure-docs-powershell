---
external help file: 
Module Name: Az.Orbital
online version: https://learn.microsoft.com/powershell/module/az.orbital/new-azorbitalspacecraft
schema: 2.0.0
content_git_url: https://github.com/Azure/azure-powershell/blob/main/src/Orbital/help/New-AzOrbitalSpacecraft.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/main/src/Orbital/help/New-AzOrbitalSpacecraft.md
---

# New-AzOrbitalSpacecraft

## SYNOPSIS
Creates or updates a spacecraft resource.

## SYNTAX

```
New-AzOrbitalSpacecraft -Name <String> -ResourceGroupName <String> -Location <String>
 [-SubscriptionId <String>] [-Link <ISpacecraftLink[]>] [-NoradId <String>] [-Tag <Hashtable>]
 [-TitleLine <String>] [-TleLine1 <String>] [-TleLine2 <String>] [-DefaultProfile <PSObject>] [-AsJob]
 [-NoWait] [-Confirm] [-WhatIf] [<CommonParameters>]
```

## DESCRIPTION
Creates or updates a spacecraft resource.

## EXAMPLES

### Example 1: Creates or updates a spacecraft resource.
```powershell
$linkObject = New-AzOrbitalSpacecraftLinkObject -BandwidthMHz 15 -CenterFrequencyMHz 8160 -Direction 'Downlink' -Name spacecraftlink -Polarization 'RHCP'

New-AzOrbitalSpacecraft -Name AQUA -ResourceGroupName azpstest-gp -Location westus2 -Link $linkObject -NoradId 27424 -TitleLine "AQUA" -TleLine1 "1 27424U 02022A   21259.45143715  .00000131  00000-0  39210-4 0  9998" -TleLine2 "2 27424  98.2138 199.4906 0001886  51.3958  60.0011 14.57112434 30322"
```

```output
Name Location NoradId TitleLine ResourceGroupName
---- -------- ------- --------- -----------------
AQUA westus2  27424   AQUA      azpstest-gp
```

Creates or updates a spacecraft resource.

## PARAMETERS

### -AsJob
Run the command as a job

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
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

### -Link
Immutable list of Spacecraft links.
To construct, see NOTES section for LINK properties and create a hash table.

```yaml
Type: Microsoft.Azure.PowerShell.Cmdlets.Orbital.Models.Api20220301.ISpacecraftLink[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Location
The geo-location where the resource lives

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

### -Name
Spacecraft ID.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases: SpacecraftName

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NoradId
NORAD ID of the spacecraft.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NoWait
Run the command asynchronously

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

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
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: (Get-AzContext).Subscription.Id
Accept pipeline input: False
Accept wildcard characters: False
```

### -Tag
Resource tags.

```yaml
Type: System.Collections.Hashtable
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TitleLine
Title line of the two-line element set (TLE).

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TleLine1
Line 1 of the two-line element set (TLE).

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TleLine2
Line 2 of the two-line element set (TLE).

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
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

### Microsoft.Azure.PowerShell.Cmdlets.Orbital.Models.Api20220301.ISpacecraft

## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


`LINK <ISpacecraftLink[]>`: Immutable list of Spacecraft links.
  - `BandwidthMHz <Single>`: Bandwidth in MHz.
  - `CenterFrequencyMHz <Single>`: Center Frequency in MHz.
  - `Direction <Direction>`: Direction (uplink or downlink).
  - `Name <String>`: Link name.
  - `Polarization <Polarization>`: Polarization. e.g. (RHCP, LHCP).

## RELATED LINKS

