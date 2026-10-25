---
title: "Asn.BookingType"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Asn 필드. 할당의 예약 유형"
type: docs
weight: 140
url: /ko/net/aspose.tasks/asn/bookingtype/
---
## Asn.BookingType field

과제의 예약 유형.

```csharp
public static readonly Key<BookingType, AsnKey> BookingType;
```

## 예제

Asn.BookingType 속성을 읽고 쓰는 방법을 보여줍니다.

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

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [BookingType](../../bookingtype/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


