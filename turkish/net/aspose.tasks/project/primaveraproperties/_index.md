---
title: "Project.PrimaveraProperties"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Project özelliği. Primavera dosyasından okunan bir proje için Primaveraspecific özellikleri içeren bir nesneyi alır."
type: docs
weight: 720
url: /tr/net/aspose.tasks/project/primaveraproperties/
---
## Project.PrimaveraProperties property

Primavera dosyasından okunan bir proje için Primavera'ya özgü özellikleri içeren bir nesne alır.

```csharp
public PrimaveraProjectProperties PrimaveraProperties { get; }
```

## Örnekler

Bir projeyi Primavera dosyasından nasıl okuyacağınızı ve projenin Primavera-specific özelliklerini nasıl inceleyeceğinizi gösterir.

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 4861;

// Özel UID'ye sahip projeyi döndürür
var project = new Project(DataDir + "ScheduleOptions.xer", options);

// PrimaveraProperties, projenin zaman çizelgesi seçenekleri varsayılan değerlerde ise null olabilir.
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

### Ayrıca Bakınız

* class [PrimaveraProjectProperties](../../primaveraprojectproperties/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


