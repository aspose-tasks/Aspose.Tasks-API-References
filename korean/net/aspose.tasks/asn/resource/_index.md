---
title: "Asn.Resource"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Asn 필드. 작업에 할당된 리소스"
type: docs
weight: 470
url: /ko/net/aspose.tasks/asn/resource/
---
## Asn.Resource field

작업에 할당된 리소스.

```csharp
public static readonly Key<Resource, AsnKey> Resource;
```

## 예제

Asn.Task 및 Asn.Resource 속성을 읽는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine("Assigned Task Name: " + assignment.Get(Asn.Task).Get(Tsk.Name));
Console.WriteLine("Assigned Resource Name: " + assignment.Get(Asn.Resource).Get(Rsc.Name));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Resource](../../resource/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


