---
title: "Asn.BookingType"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Asn alanı. Bir atamanın rezervasyon türü"
type: docs
weight: 140
url: /tr/net/aspose.tasks/asn/bookingtype/
---
## Asn.BookingType field

Bir atamanın rezervasyon türü.

```csharp
public static readonly Key<BookingType, AsnKey> BookingType;
```

## Örnekler

Asn.BookingType özelliğini okuma/yazma nasıl yapılır gösterir.

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

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [BookingType](../../bookingtype/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


