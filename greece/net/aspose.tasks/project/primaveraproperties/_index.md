---
title: "Project.PrimaveraProperties"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Project. Λαμβάνει ένα αντικείμενο που περιέχει ιδιότητες ειδικές για Primavera για ένα έργο που διαβάστηκε από αρχείο Primavera."
type: docs
weight: 720
url: /el/net/aspose.tasks/project/primaveraproperties/
---
## Project.PrimaveraProperties property

Λαμβάνει ένα αντικείμενο που περιέχει ιδιότητες ειδικές για Primavera για ένα έργο που διαβάστηκε από αρχείο Primavera.

```csharp
public PrimaveraProjectProperties PrimaveraProperties { get; }
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε ένα έργο από αρχείο Primavera και να εξετάσετε τις ιδιότητες ειδικές για Primavera του έργου.

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 4861;

// Επιστρέφει έργο με ειδικό UID
var project = new Project(DataDir + "ScheduleOptions.xer", options);

// Το PrimaveraProperties μπορεί να είναι null εάν οι επιλογές χρονοδιαγράμματος του έργου έχουν προεπιλεγμένες τιμές.
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

### Δείτε επίσης

* class [PrimaveraProjectProperties](../../primaveraprojectproperties/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


