---
title: "Project.PrimaveraProperties"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Project. Mendapatkan objek yang berisi properti Primaveraspecific untuk sebuah proyek yang dibaca dari file Primavera."
type: docs
weight: 720
url: /id/net/aspose.tasks/project/primaveraproperties/
---
## Project.PrimaveraProperties property

Mendapatkan objek yang berisi properti khusus Primavera untuk sebuah proyek yang dibaca dari file Primavera.

```csharp
public PrimaveraProjectProperties PrimaveraProperties { get; }
```

## Contoh

Menampilkan cara membaca proyek dari file Primavera dan memeriksa properti khusus Primavera proyek tersebut.

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 4861;

// Mengembalikan proyek dengan UID khusus
var project = new Project(DataDir + "ScheduleOptions.xer", options);

// PrimaveraProperties dapat bernilai null jika opsi jadwal proyek memiliki nilai default.
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

### Lihat Juga

* class [PrimaveraProjectProperties](../../primaveraprojectproperties/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


