---
title: "Asn.BookingType"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Asn-veld. Het boekingssoort van een toewijzing"
type: docs
weight: 140
url: /nl/net/aspose.tasks/asn/bookingtype/
---
## Asn.BookingType field

Het boekingstype van een opdracht.

```csharp
public static readonly Key<BookingType, AsnKey> BookingType;
```

## Voorbeelden

Toont hoe de eigenschap Asn.BookingType te lezen/schrijven.

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

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [BookingType](../../bookingtype/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


