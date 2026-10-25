---
title: "Απαρίθμηση BookingType"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Απαρίθμηση Aspose.Tasks.BookingType. Καθορίζει τον τύπο κράτησης ενός πόρου."
type: docs
weight: 150
url: /el/net/aspose.tasks/bookingtype/
---
## BookingType enumeration

Καθορίζει τον τύπο κράτησης ενός πόρου.

```csharp
public enum BookingType
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| Undefined | `-1` | Δείχνει ότι η τιμή δεν ορίστηκε στο αρχικό αρχείο έργου. |
| Committed | `0` | Δείχνει τον τύπο κράτησης Committed. |
| Proposed | `1` | Δείχνει τον τύπο κράτησης Proposed. |

## Παρατηρήσεις

Κατά την εξαγωγή σε XML, οι μη ορισμένες τιμές θα αφαιρεθούν από το τελικό XML.

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Asn.BookingType.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.BookingType, BookingType.Proposed);

Console.WriteLine("Booking Type: " + assignment.Get(Asn.BookingType));
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


