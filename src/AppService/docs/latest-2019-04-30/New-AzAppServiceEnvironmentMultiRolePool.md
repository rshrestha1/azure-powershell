---
external help file:
Module Name: Az.WebSite
online version: https://docs.microsoft.com/en-us/powershell/module/az.website/new-azappserviceenvironmentmultirolepool
schema: 2.0.0
---

# New-AzAppServiceEnvironmentMultiRolePool

## SYNOPSIS
Create or update a multi-role pool.

## SYNTAX

### Create (Default)
```
New-AzAppServiceEnvironmentMultiRolePool -Name <String> -ResourceGroupName <String> -SubscriptionId <String>
 [-MultiRolePoolEnvelope <IWorkerPoolResource>] [-PassThru] [-DefaultProfile <PSObject>] [-AsJob] [-NoWait]
 [-Confirm] [-WhatIf] [<CommonParameters>]
```

### CreateExpanded
```
New-AzAppServiceEnvironmentMultiRolePool -Name <String> -ResourceGroupName <String> -SubscriptionId <String>
 [-PassThru] [-Capacity <Int32>] [-ComputeMode <ComputeModeOptions>] [-Kind <String>]
 [-SkuCapability <ICapability[]>] [-SkuCapacityDefault <Int32>] [-SkuCapacityMaximum <Int32>]
 [-SkuCapacityMinimum <Int32>] [-SkuCapacityScaleType <String>] [-SkuFamily <String>]
 [-SkuLocation <String[]>] [-SkuName <String>] [-SkuSize <String>] [-SkuTier <String>] [-WorkerCount <Int32>]
 [-WorkerSize <String>] [-WorkerSizeId <Int32>] [-DefaultProfile <PSObject>] [-AsJob] [-NoWait] [-Confirm]
 [-WhatIf] [<CommonParameters>]
```

### CreateViaIdentityExpanded
```
New-AzAppServiceEnvironmentMultiRolePool -InputObject <IWebSiteIdentity> [-PassThru] [-Capacity <Int32>]
 [-ComputeMode <ComputeModeOptions>] [-Kind <String>] [-SkuCapability <ICapability[]>]
 [-SkuCapacityDefault <Int32>] [-SkuCapacityMaximum <Int32>] [-SkuCapacityMinimum <Int32>]
 [-SkuCapacityScaleType <String>] [-SkuFamily <String>] [-SkuLocation <String[]>] [-SkuName <String>]
 [-SkuSize <String>] [-SkuTier <String>] [-WorkerCount <Int32>] [-WorkerSize <String>] [-WorkerSizeId <Int32>]
 [-DefaultProfile <PSObject>] [-AsJob] [-NoWait] [-Confirm] [-WhatIf] [<CommonParameters>]
```

### CreateViaIdentity
```
New-AzAppServiceEnvironmentMultiRolePool -InputObject <IWebSiteIdentity>
 [-MultiRolePoolEnvelope <IWorkerPoolResource>] [-PassThru] [-DefaultProfile <PSObject>] [-AsJob] [-NoWait]
 [-Confirm] [-WhatIf] [<CommonParameters>]
```

## DESCRIPTION
Create or update a multi-role pool.

## EXAMPLES

### Example 1: {{ Add title here }}
```powershell
PS C:\> {{ Add code here }}

{{ Add output here }}
```

{{ Add description here }}

### Example 2: {{ Add title here }}
```powershell
PS C:\> {{ Add code here }}

{{ Add output here }}
```

{{ Add description here }}

## PARAMETERS

### -AsJob
Run the command as a job

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -Capacity
Current number of instances assigned to the resource.

```yaml
Type: System.Int32
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -ComputeMode
Shared or dedicated app hosting.

```yaml
Type: Microsoft.Azure.PowerShell.Cmdlets.WebSite.Support.ComputeModeOptions
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
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
Dynamic: False
```

### -InputObject
Identity Parameter

```yaml
Type: Microsoft.Azure.PowerShell.Cmdlets.WebSite.Models.IWebSiteIdentity
Parameter Sets: CreateViaIdentityExpanded, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
Dynamic: False
```

### -Kind
Kind of resource.

```yaml
Type: System.String
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -MultiRolePoolEnvelope
Worker pool of an App Service Environment ARM resource.
To construct, see NOTES section for MULTIROLEPOOLENVELOPE properties and create a hash table.

```yaml
Type: Microsoft.Azure.PowerShell.Cmdlets.WebSite.Models.Api20160901.IWorkerPoolResource
Parameter Sets: Create, CreateViaIdentity
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
Dynamic: False
```

### -Name
Name of the App Service Environment.

```yaml
Type: System.String
Parameter Sets: Create, CreateExpanded
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -NoWait
Run the command asynchronously

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -PassThru
When specified, PassThru will force the cmdlet return a 'bool' given that there isn't a return type by default.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -ResourceGroupName
Name of the resource group to which the resource belongs.

```yaml
Type: System.String
Parameter Sets: Create, CreateExpanded
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -SkuCapability
Capabilities of the SKU, e.g., is traffic manager enabled
To construct, see NOTES section for SKUCAPABILITY properties and create a hash table.

```yaml
Type: Microsoft.Azure.PowerShell.Cmdlets.WebSite.Models.Api20160301.ICapability[]
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -SkuCapacityDefault
Default number of workers for this App Service plan SKU.

```yaml
Type: System.Int32
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -SkuCapacityMaximum
Maximum number of workers for this App Service plan SKU.

```yaml
Type: System.Int32
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -SkuCapacityMinimum
Minimum number of workers for this App Service plan SKU.

```yaml
Type: System.Int32
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -SkuCapacityScaleType
Available scale configurations for an App Service plan.

```yaml
Type: System.String
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -SkuFamily
Family code of the resource SKU.

```yaml
Type: System.String
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -SkuLocation
Locations of the SKU.

```yaml
Type: System.String[]
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -SkuName
Name of the resource SKU.

```yaml
Type: System.String
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -SkuSize
Size specifier of the resource SKU.

```yaml
Type: System.String
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -SkuTier
Service tier of the resource SKU.

```yaml
Type: System.String
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -SubscriptionId
Your Azure subscription ID.
This is a GUID-formatted string (e.g.
00000000-0000-0000-0000-000000000000).

```yaml
Type: System.String
Parameter Sets: Create, CreateExpanded
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -WorkerCount
Number of instances in the worker pool.

```yaml
Type: System.Int32
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -WorkerSize
VM size of the worker pool instances.

```yaml
Type: System.String
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -WorkerSizeId
Worker size ID for referencing this worker pool.

```yaml
Type: System.Int32
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
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
Dynamic: False
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
Dynamic: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Azure.PowerShell.Cmdlets.WebSite.Models.IWebSiteIdentity

### Microsoft.Azure.PowerShell.Cmdlets.WebSite.Models.Api20160901.IWorkerPoolResource

## OUTPUTS

### Microsoft.Azure.PowerShell.Cmdlets.WebSite.Models.Api20160901.IWorkerPoolResource

## ALIASES

## NOTES

### COMPLEX PARAMETER PROPERTIES
To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.

#### MULTIROLEPOOLENVELOPE <IWorkerPoolResource>: Worker pool of an App Service Environment ARM resource.
  - `[Kind <String>]`: Kind of resource.
  - `[Capacity <Int32?>]`: Current number of instances assigned to the resource.
  - `[ComputeMode <ComputeModeOptions?>]`: Shared or dedicated app hosting.
  - `[SkuCapability <ICapability[]>]`: Capabilities of the SKU, e.g., is traffic manager enabled?
    - `[Name <String>]`: Name of the SKU capability.
    - `[Reason <String>]`: Reason of the SKU capability.
    - `[Value <String>]`: Value of the SKU capability.
  - `[SkuCapacityDefault <Int32?>]`: Default number of workers for this App Service plan SKU.
  - `[SkuCapacityMaximum <Int32?>]`: Maximum number of workers for this App Service plan SKU.
  - `[SkuCapacityMinimum <Int32?>]`: Minimum number of workers for this App Service plan SKU.
  - `[SkuCapacityScaleType <String>]`: Available scale configurations for an App Service plan.
  - `[SkuFamily <String>]`: Family code of the resource SKU.
  - `[SkuLocation <String[]>]`: Locations of the SKU.
  - `[SkuName <String>]`: Name of the resource SKU.
  - `[SkuSize <String>]`: Size specifier of the resource SKU.
  - `[SkuTier <String>]`: Service tier of the resource SKU.
  - `[WorkerCount <Int32?>]`: Number of instances in the worker pool.
  - `[WorkerSize <String>]`: VM size of the worker pool instances.
  - `[WorkerSizeId <Int32?>]`: Worker size ID for referencing this worker pool.

#### SKUCAPABILITY <ICapability[]>: Capabilities of the SKU, e.g., is traffic manager enabled
  - `[Name <String>]`: Name of the SKU capability.
  - `[Reason <String>]`: Reason of the SKU capability.
  - `[Value <String>]`: Value of the SKU capability.

## RELATED LINKS
