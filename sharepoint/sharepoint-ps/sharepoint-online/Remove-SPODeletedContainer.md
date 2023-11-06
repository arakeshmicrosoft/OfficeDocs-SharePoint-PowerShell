---
external help file: sharepointonline.xml
Module Name: Microsoft.Online.SharePoint.PowerShell
online version: 
applicable: SharePoint Online
title: Remove-SPOContainerDeletedContainer
schema: 2.0.0
author: cindy-lay
ms.author: cindylay
ms.reviewer:
---


# Remove-SPODeletedContainer



## SYNOPSIS

Permanently deletes the specified SharePoint Embedded container from the deleted container collection if the Container has no further retention policies applied to it. This action cannot be undone.

> [!WARNING]
> Deleting a container may cause unexpected issues for the SharePoint Embedded application the Container belongs to and may interrupt usage of the application.

## SYNTAX



### ParamSet1

```powershell
Remove-SPODeletedContainer [–Identity <ContainerID>] [<CommonParameters>]
```

## DESCRIPTION

The `Remove-SPODeletedContainer` cmdlet permanently removes a SharePoint Embedded deleted container from the deleted container collection.

You must be a SharePoint Administrator or Global Administrator to run the cmdlet. To get started using PowerShell to manage SharePoint Embedded, you have to [install](https://www.microsoft.com/en-us/download/details.aspx?id=35588) the SharePoint Online Management Shell and [connect to SharePoint Online](https://learn.microsoft.com/en-us/powershell/module/sharepoint-online/connect-sposervice?view=sharepoint-ps). 

You need version 16.0.24211.12000 or higher to run the commands for SharePoint Embedded.

## EXAMPLES

### -----------------------EXAMPLE 1-----------------------------

```powershell
Remove-SPODeletedContainer –Identity b!66f5b2e-4cbd-4754-9ad3-8291c2c81ade
``````
This example removes a SharePoint Embedded deleted container with the ContainerID b!66f5b2e-4cbd-4754-9ad3-8291c2c81adefrom the deleted cointainer collection and deletes it permanently.

## PARAMETERS


### -Identity

Specifies the `<ContainerID>`of the Container to be permanently deleted.
 
```yaml
Type: String
Parameter Sets: (All)
Aliases:
Applicable: SharePoint Online

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```


### CommonParameters

This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](https://go.microsoft.com/fwlink/?LinkID=113216).


## INPUTS

### Microsoft.Online.SharePoint.PowerShell.SpoSitePipeBind

## OUTPUTS

### System.Object

## NOTES

## RELATED LINKS

[Getting started with SharePoint Online Management Shell](https://learn.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)

[Remove-SPOContainer](Remove-SPOContainer.md)

