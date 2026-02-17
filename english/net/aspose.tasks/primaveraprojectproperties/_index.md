---
title: Class PrimaveraProjectProperties
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.PrimaveraProjectProperties class. Represents Primaveraspecific properties for a project read from Primavera files XER of P6XML
type: docs
weight: 1350
url: /net/aspose.tasks/primaveraprojectproperties/
---
## PrimaveraProjectProperties class

Represents Primavera-specific properties for a project read from Primavera files (XER of P6XML).

```csharp
public sealed class PrimaveraProjectProperties
```

## Properties

| Name | Description |
| --- | --- |
| [BaselineProjects](../../aspose.tasks/primaveraprojectproperties/baselineprojects/) { get; } | Gets array of baseline projects of current project. Is applicable to projects read from Primavera XML files containing exported baselines. |
| [CriticalActivitiesDefiningMethod](../../aspose.tasks/primaveraprojectproperties/criticalactivitiesdefiningmethod/) { get; } | Gets the method for defining critical activities: Longest Path or Total Float approach. |
| [CriticalTotalFloatLimit](../../aspose.tasks/primaveraprojectproperties/criticaltotalfloatlimit/) { get; } | Gets the threshold value used to define critical activities if TotalFloat method is used. |
| [CurrentBaselineProjectId](../../aspose.tasks/primaveraprojectproperties/currentbaselineprojectid/) { get; } | Gets Id of the current baseline project. Is applicable to projects read from Primavera XML files containing exported baselines. |
| [IgnoreOtherProjectRelationships](../../aspose.tasks/primaveraprojectproperties/ignoreotherprojectrelationships/) { get; } | Gets a flag which defines whether to ignore activity relationships between projects. |
| [MakeOpenEndedActivitiesCritical](../../aspose.tasks/primaveraprojectproperties/makeopenendedactivitiescritical/) { get; } | Gets a flag which defines whether activities should me marked as critical when scheduling the project. |
| [RelationshipLagCalendar](../../aspose.tasks/primaveraprojectproperties/relationshiplagcalendar/) { get; } | Gets an options which defines which calendar to use for scheduling Relationship Lag in Primavera projects |
| [ShortName](../../aspose.tasks/primaveraprojectproperties/shortname/) { get; } | Gets project's short name (Project ID). |
| [UseExpectedFinishDates](../../aspose.tasks/primaveraprojectproperties/useexpectedfinishdates/) { get; } | Gets a flag which defines whether activity finish dates should be scheduled as the expected finish dates. |

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


