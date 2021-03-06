# Remove-vRAUserPrincipal

## SYNOPSIS
    
Remove a vRA local user principal

## SYNTAX
 Remove-vRAUserPrincipal [-Id] <String[]> [[-Tenant] <String>] [-WhatIf] [-Confirm] [<CommonParameters>]     

## DESCRIPTION

Remove a vRA local user principal

## PARAMETERS


### Id

The principal id of the user

* Required: true
* Position: 1
* Default value: 
* Accept pipeline input: true (ByValue, ByPropertyName)

### Tenant

The tenant of the user

* Required: false
* Position: 2
* Default value: $Global:vRAConnection.Tenant
* Accept pipeline input: false

### WhatIf


* Required: false
* Position: named
* Default value: 
* Accept pipeline input: false

### Confirm


* Required: false
* Position: named
* Default value: 
* Accept pipeline input: false

## INPUTS

System.String.

## OUTPUTS

None

## EXAMPLES
```
-------------------------- EXAMPLE 1 --------------------------

PS C:\>Remove-vRAUserPrincipal -PrincipalId user@vsphere.local






-------------------------- EXAMPLE 2 --------------------------

PS C:\>Get-vRAUserPrincipal -Id user@vsphere.local | Remove-vRAUserPrincipal
```

