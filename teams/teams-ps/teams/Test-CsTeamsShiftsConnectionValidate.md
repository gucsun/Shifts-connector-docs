---
external help file: Microsoft.TeamsCmdlets.PowerShell.Custom.dll-Help.xml
Module Name: MicrosoftTeams
title: Test-CsTeamsShiftsConnectionValidate
author: gucsun
manager: navinth
online version: https://docs.microsoft.com/powershell/module/teams/Test-CsTeamsShiftsConnectionValidate
schema: 2.3.4
---

# Test-CsTeamsShiftsConnectionValidate

## SYNOPSIS

**Note:** This cmdlet is currently in private preview.

This cmdlet validates WFM settings from given configuration.

## SYNTAX

```
Test-CsTeamsShiftsConnectionValidate -ConnectorId <string> -ConnectorSpecificSettingAdminApiUrl <string> -ConnectorSpecificSettingCookieAuthUrl <string> -ConnectorSpecificSettingEssApiUrl <string> -ConnectorSpecificSettingFederatedAuthUrl <string> -ConnectorSpecificSettingLoginPwd <string> -ConnectorSpecificSettingLoginUserName <string> -ConnectorSpecificSettingRetailWebApiUrl <string> -ConnectorSpecificSettingSiteManagerUrl <string> -Name <string> [<CommonParameters>]
```

## DESCRIPTION

This cmdlet allows the admin to test if there are conflicts to create an instance with the input settings.

## EXAMPLES

### Example 1
```powershell
PS C:\> $InstanceName = "test instance name"
PS C:\> $WfmUserName = "WfmUserName"
PS C:\> $plainPwd = "plainPwd"
PS C:\> Test-CsTeamsShiftsConnectionValidate -ConnectorId "6A51B888-FF44-4FEA-82E1-839401E9CD74" -ConnectorSpecificSettingAdminApiUrl "https://nehstdevwfm02.replgroup.com/retail/data/wfmadmin/api/v1-beta2" -ConnectorSpecificSettingCookieAuthUrl "https://nehstdevwfm02.replgroup.com/retail/data/login" -ConnectorSpecificSettingEssApiUrl "https://nehstdevfas01.replgroup.com/retail/data/wfmess/api/v1-beta1" -ConnectorSpecificSettingFederatedAuthUrl "https://nehstdevfas01.replgroup.com/retail/data/login" -ConnectorSpecificSettingLoginPwd $plainPwd -ConnectorSpecificSettingLoginUserName $WfmUserName -ConnectorSpecificSettingRetailWebApiUrl "https://nehstdevwfm02.replgroup.com/retail/data/retailwebapi/api/v1" -ConnectorSpecificSettingSiteManagerUrl "https://nehstdevfas01.replgroup.com/retail/data/wfmsm/api/v1-beta2" -Name $InstanceName
```

Returns the list of conflicts if there are any. Empty result means there's no conflict.

## PARAMETERS

### -ConnectorId

The ID of the shifts connector.

```yaml
Type: String
Parameter Sets: (All)
Aliases:
Applicable: Microsoft Teams
Required: True
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name

The connector's instance name.

```yaml
Type: String
Parameter Sets: (All)
Aliases:
Applicable: Microsoft Teams
Required: True
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ConnectorSpecificSettingLoginUserName

The login user name to WFM team.

```yaml
Type: String
Parameter Sets: (All)
Aliases:
Applicable: Microsoft Teams
Required: True
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ConnectorSpecificSettingLoginPwd

The login password to WFM team.

```yaml
Type: String
Parameter Sets: (All)
Aliases:
Applicable: Microsoft Teams
Required: True
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ConnectorSpecificSettingAdminApiUrl

The admin api URL.

```yaml
Type: String
Parameter Sets: (All)
Aliases:
Applicable: Microsoft Teams
Required: True
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ConnectorSpecificSettingCookieAuthUrl

The cookie authorization URL.

```yaml
Type: String
Parameter Sets: (All)
Aliases:
Applicable: Microsoft Teams
Required: True
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ConnectorSpecificSettingEssApiUrl

The essential api URL.

```yaml
Type: String
Parameter Sets: (All)
Aliases:
Applicable: Microsoft Teams
Required: True
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ConnectorSpecificSettingFederatedAuthUrl

The federated authorization URL.

```yaml
Type: String
Parameter Sets: (All)
Aliases:
Applicable: Microsoft Teams
Required: True
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ConnectorSpecificSettingRetailWebApiUrl

The retail web api URL.

```yaml
Type: String
Parameter Sets: (All)
Aliases:
Applicable: Microsoft Teams
Required: True
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ConnectorSpecificSettingSiteManagerUrl

The site manager URL.

```yaml
Type: String
Parameter Sets: (All)
Aliases:
Applicable: Microsoft Teams
Required: True
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

[New-CsTeamsShiftsConnectionInstance](New-CsTeamsShiftsConnectionInstance.md)

[Set-CsTeamsShiftsConnectionInstance](Set-CsTeamsShiftsConnectionInstance.md)
