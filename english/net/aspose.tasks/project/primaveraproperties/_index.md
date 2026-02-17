---
title: Project.PrimaveraProperties
second_title: Aspose.Tasks for .NET API Reference
description: Project property. Gets an object containing Primaveraspecific properties for a project read from Primavera file
type: docs
weight: 720
url: /net/aspose.tasks/project/primaveraproperties/
---
## Project.PrimaveraProperties property

Gets an object containing Primavera-specific properties for a project read from Primavera file.

```csharp
public PrimaveraProjectProperties PrimaveraProperties { get; }
```

## Examples

Shows how to read a project from a Primavera file and examine project's Primavera-specific properties.

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 4861;

// Returns project with special Uid
var project = new Project(DataDir + "ScheduleOptions.xer", options);

// PrimaveraProperties can be null if project's schedule options have default values.
if (project.PrimaveraProperties != null)
{
    Console.WriteLine("Project's schedule options:");
    Console.WriteLine("Relationship Lag Calendar: " + project.PrimaveraProperties.RelationshipLagCalendar);
    Console.WriteLine("Make Open Ended Activities Critical: " + project.PrimaveraProperties.MakeOpenEndedActivitiesCritical);
    Console.WriteLine("Ignore Other Project Relationships: " + project.PrimaveraProperties.IgnoreOtherProjectRelationships);
    Console.WriteLine("Use Expected Finish Dates: " + project.PrimaveraProperties.UseExpectedFinishDates);

    Console.WriteLine("How critical activities are defined: " +
                      project.PrimaveraProperties.CriticalActivitiesDefiningMethod);

    if (project.PrimaveraProperties.CriticalActivitiesDefiningMethod == PrimaveraCriticalActivitiesDefiningMethod.TotalFloat)
    {
        Console.WriteLine("Total Float threshold for critical activities: " + project.PrimaveraProperties.CriticalTotalFloatLimit);
    }
}
```

### See Also

* class [PrimaveraProjectProperties](../../primaveraprojectproperties/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


