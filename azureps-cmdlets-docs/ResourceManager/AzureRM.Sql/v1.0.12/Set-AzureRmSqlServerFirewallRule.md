---
external help file: Microsoft.Azure.Commands.Sql.dll-Help.xml
online version: .\Get-AzureRmSqlServerFirewallRule.md
schema: 2.0.0
ms.assetid: 8ED6F48C-5480-4C24-A3CE-6A7EE6D29FB4
---

# Set-AzureRmSqlServerFirewallRule

## SYNOPSIS
Modifies a firewall rule in ssSDS server.

## SYNTAX

```
Set-AzureRmSqlServerFirewallRule [-FirewallRuleName] <String> -StartIpAddress <String> -EndIpAddress <String>
 [-ServerName] <String> [-ResourceGroupName] <String> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Set-AzureRmSqlServerFirewallRule** cmdlet modifies a firewall rule in an ssSDS server.

## EXAMPLES

### Example 1: Modify a firewall rule
```
PS C:\>Set-AzureRmSqlServerFirewallRule -ResourceGroupName "ResourceGroup01" -ServerName "Server01" -FirewallRuleName "Rule01" -StartIpAddress "192.168.0.197" -EndIpAddress "192.168.0.199"
ResourceGroupName : ResourceGroup01
ServerName        : Server01
StartIpAddress    : 192.168.0.199
EndIpAddress      : 192.168.0.200
FirewallRuleName  : Rule01
```

This command modifies a firewall rule named Rule01 on the server named Server01.
The command modifies the start and end IP addresses.

## PARAMETERS

### -FirewallRuleName
Specifies the name of the firewall rule that this cmdlet modifies.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -StartIpAddress
Specifies the start value of the IP address range for the firewall rule.

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

### -EndIpAddress
Specifies the end value of the IP address range for this rule.

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

### -ServerName
Specifies the name of the server.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of the resource group to which the server is assigned.

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

### -InformationAction
Specifies how this cmdlet responds to an information event.

The acceptable values for this parameter are:

- Continue
- Ignore
- Inquire
- SilentlyContinue
- Stop
- Suspend

```yaml
Type: ActionPreference
Parameter Sets: (All)
Aliases: infa

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationVariable
Specifies an information variable.

```yaml
Type: String
Parameter Sets: (All)
Aliases: iv

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

### Microsoft.Azure.Commands.Sql.FirewallRule.Model.AzureSqlServerFirewallRuleModel

## NOTES

## RELATED LINKS

[Get-AzureRmSqlServerFirewallRule](./Get-AzureRmSqlServerFirewallRule.md)

[New-AzureRmSqlServerFirewallRule](./New-AzureRmSqlServerFirewallRule.md)

[Remove-AzureRmSqlServerFirewallRule](./Remove-AzureRmSqlServerFirewallRule.md)

[Azure SQL Database Cmdlets](./AzureRM.Sql.md)

