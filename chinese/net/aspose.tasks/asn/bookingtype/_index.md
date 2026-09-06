---
title: "Asn.BookingType"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Asn 字段。任务的预订类型"
type: docs
weight: 140
url: /zh/net/aspose.tasks/asn/bookingtype/
---
## Asn.BookingType field

任务的预订类型。

```csharp
public static readonly Key<BookingType, AsnKey> BookingType;
```

## 示例

展示如何读取/写入 Asn.BookingType 属性。

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

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [BookingType](../../bookingtype/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


