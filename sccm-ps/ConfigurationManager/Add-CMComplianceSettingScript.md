---
external help file: AdminUI.PS.Dcm.dll-Help.xml
online version: 
schema: 2.0.0
---

# Add-CMComplianceSettingScript

## SYNOPSIS
Adds a compliance setting script

## SYNTAX

### EmptyRule (Default)
```
Add-CMComplianceSettingScript -DataType <SettingDataType> [-DiscoveryScriptFile <String>]
 -DiscoveryScriptLanguage <ScriptingLanguage> [-DiscoveryScriptText <String>] [-Is64Bit] [-IsPerUser]
 [-RemediationScriptFile <String>] [-RemediationScriptLanguage <ScriptingLanguage>]
 [-RemediationScriptText <String>] [-Description <String>] -InputObject <PSObject> -Name <String> [-NoRule]
 [-PassThru] [-DisableWildcardHandling] [-ForceWildcardHandling] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### ExistentialRule
```
Add-CMComplianceSettingScript -DataType <SettingDataType> [-DiscoveryScriptFile <String>]
 -DiscoveryScriptLanguage <ScriptingLanguage> [-DiscoveryScriptText <String>] [-Is64Bit] [-IsPerUser]
 [-RemediationScriptFile <String>] [-RemediationScriptLanguage <ScriptingLanguage>]
 [-RemediationScriptText <String>] [-Description <String>] -Existence <ExistenceType> [-ExistentialRule]
 [-ExpectedValue <String[]>] [-ExpressionOperator <RuleExpressionOperator>] -InputObject <PSObject>
 -Name <String> [-NoncomplianceSeverity <NoncomplianceSeverity>] [-RuleDescription <String>] -RuleName <String>
 [-PassThru] [-DisableWildcardHandling] [-ForceWildcardHandling] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### ValueRule
```
Add-CMComplianceSettingScript -DataType <SettingDataType> [-DiscoveryScriptFile <String>]
 -DiscoveryScriptLanguage <ScriptingLanguage> [-DiscoveryScriptText <String>] [-Is64Bit] [-IsPerUser]
 [-RemediationScriptFile <String>] [-RemediationScriptLanguage <ScriptingLanguage>]
 [-RemediationScriptText <String>] [-Description <String>] -ExpectedValue <String[]>
 -ExpressionOperator <RuleExpressionOperator> -InputObject <PSObject> -Name <String>
 [-NoncomplianceSeverity <NoncomplianceSeverity>] [-ReportNoncompliance] [-RuleDescription <String>]
 -RuleName <String> [-ValueRule] [-PassThru] [-DisableWildcardHandling] [-ForceWildcardHandling] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
{{Fill in the Description}}

## EXAMPLES

### Example 1
```
PS C:\> {{ Add example code here }}
```

{{ Add example description here }}

## PARAMETERS

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

### -DataType
{{Fill DataType Description}}

```yaml
Type: SettingDataType
Parameter Sets: (All)
Aliases: 
Accepted values: String, DateTime, Integer, FloatingPoint, Version, Boolean

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Description
{{Fill Description Description}}

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

### -DisableWildcardHandling
DisableWildcardHandling treats wildcard characters as literal character values. Cannot be combined with **ForceWildcardHandling**.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DiscoveryScriptFile
{{Fill DiscoveryScriptFile Description}}

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

### -DiscoveryScriptLanguage
{{Fill DiscoveryScriptLanguage Description}}

```yaml
Type: ScriptingLanguage
Parameter Sets: (All)
Aliases: 
Accepted values: PowerShell, VBScript, JScript, ShellScript

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DiscoveryScriptText
{{Fill DiscoveryScriptText Description}}

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

### -Existence
{{Fill Existence Description}}

```yaml
Type: ExistenceType
Parameter Sets: ExistentialRule
Aliases: 
Accepted values: MustExist, MustNotExist, Occurs

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExistentialRule
{{Fill ExistentialRule Description}}

```yaml
Type: SwitchParameter
Parameter Sets: ExistentialRule
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExpectedValue
{{Fill ExpectedValue Description}}

```yaml
Type: String[]
Parameter Sets: ExistentialRule
Aliases: ExpectedValues, ExpectedCount, ExpectedCounts

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

```yaml
Type: String[]
Parameter Sets: ValueRule
Aliases: ExpectedValues, ExpectedCount, ExpectedCounts

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExpressionOperator
{{Fill ExpressionOperator Description}}

```yaml
Type: RuleExpressionOperator
Parameter Sets: ExistentialRule
Aliases: 
Accepted values: And, Or, Other, IsEquals, NotEquals, GreaterThan, LessThan, Between, NotBetween, GreaterEquals, LessEquals, BeginsWith, NotBeginsWith, EndsWith, NotEndsWith, Contains, NotContains, AllOf, OneOf, NoneOf, SetEquals, SubsetOf, ExcludesAll

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

```yaml
Type: RuleExpressionOperator
Parameter Sets: ValueRule
Aliases: 
Accepted values: And, Or, Other, IsEquals, NotEquals, GreaterThan, LessThan, Between, NotBetween, GreaterEquals, LessEquals, BeginsWith, NotBeginsWith, EndsWith, NotEndsWith, Contains, NotContains, AllOf, OneOf, NoneOf, SetEquals, SubsetOf, ExcludesAll

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ForceWildcardHandling
ForceWildcardHandling processes wildcard characters and may lead to unexpected behavior (not recommended). Cannot be combined with **DisableWildcardHandling**.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputObject
{{Fill InputObject Description}}

```yaml
Type: PSObject
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Is64Bit
{{Fill Is64Bit Description}}

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -IsPerUser
{{Fill IsPerUser Description}}

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
{{Fill Name Description}}

```yaml
Type: String
Parameter Sets: (All)
Aliases: SettingName

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NoRule
{{Fill NoRule Description}}

```yaml
Type: SwitchParameter
Parameter Sets: EmptyRule
Aliases: NoRules

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NoncomplianceSeverity
{{Fill NoncomplianceSeverity Description}}

```yaml
Type: NoncomplianceSeverity
Parameter Sets: ExistentialRule, ValueRule
Aliases: 
Accepted values: None, Informational, Warning, Critical, CriticalWithEvent

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PassThru
Returns an object representing the item with which you are working. By default, this cmdlet may not generate any output.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RemediationScriptFile
{{Fill RemediationScriptFile Description}}

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

### -RemediationScriptLanguage
{{Fill RemediationScriptLanguage Description}}

```yaml
Type: ScriptingLanguage
Parameter Sets: (All)
Aliases: 
Accepted values: PowerShell, VBScript, JScript, ShellScript

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RemediationScriptText
{{Fill RemediationScriptText Description}}

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

### -ReportNoncompliance
{{Fill ReportNoncompliance Description}}

```yaml
Type: SwitchParameter
Parameter Sets: ValueRule
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RuleDescription
{{Fill RuleDescription Description}}

```yaml
Type: String
Parameter Sets: ExistentialRule, ValueRule
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RuleName
{{Fill RuleName Description}}

```yaml
Type: String
Parameter Sets: ExistentialRule, ValueRule
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ValueRule
{{Fill ValueRule Description}}

```yaml
Type: SwitchParameter
Parameter Sets: ValueRule
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.Management.Automation.PSObject

## OUTPUTS

### System.Object

## NOTES

## RELATED LINKS
