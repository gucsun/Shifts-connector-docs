---
external help file: Microsoft.TeamsCmdlets.PowerShell.Custom.dll-Help.xml
Module Name: MicrosoftTeams
title: Get-CsTeamsShiftsConnectionUser
author: gucsun
manager: navinth
online version: https://docs.microsoft.com/powershell/module/teams/get-csteamsshiftsconnectionuser
schema: 2.4.0
---

# Get-CsTeamsShiftsConnectionUser

## SYNOPSIS

**Note:** This cmdlet is currently in private preview.

This cmdlet supports retrieving the list of users in the connection instance.

## SYNTAX

```
Get-CsTeamsShiftsConnectionUser -ConnectorInstanceId <string> -WfmTeamId <string> [<CommonParameters>]
```

## DESCRIPTION

This cmdlet shows the list of WFM users in the connection instance.

## EXAMPLES

### Example 1
```powershell
PS C:\> Get-CsTeamsShiftsConnectionUser -ConnectorInstanceId "WCI-4c231dd2-4451-45bd-8eea-bd68b40bab8b" -WfmTeamId "1000107"
```

Returns the users in the WFM team with ID 1000107 in the connection instances with ID WCI-2302814d-f316-4d80-91cc-11508c24d51c.

## PARAMETERS

### -ConnectorInstanceId

The ID of the connection instance. It can be retrieved by running [Get-CsTeamsShiftsConnectionInstance](Get-CsTeamsShiftsConnectionInstance.md)

```yaml
Type: String
Parameter Sets: (All)
Aliases:
Applicable: Microsoft Teams
Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WfmTeamId

The Teams team ID. It can be retrieved by running [Get-CsTeamsShiftsConnectionWfmTeam](Get-CsTeamsShiftsConnectionWfmTeam.md)

```yaml
Type: String
Parameter Sets: (All)
Aliases:
Applicable: Microsoft Teams
Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](https://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-CsTeamsShiftsConnectionInstance](Get-CsTeamsShiftsConnectionInstance.md)

[Get-CsTeamsShiftsConnectionWfmTeam](Get-CsTeamsShiftsConnectionWfmTeam.md)
