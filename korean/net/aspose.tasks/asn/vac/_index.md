---
title: "Asn.VAC"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Asn 필드. 기준 비용과 총 비용 간의 차이"
type: docs
weight: 590
url: /ko/net/aspose.tasks/asn/vac/
---
## Asn.VAC field

기준 비용과 총 비용의 차이.

```csharp
public static readonly Key<double, AsnKey> VAC;
```

## 예제

Asn.VAC 속성을 읽는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.VAC, 10);

Console.WriteLine("VAC: " + assignment.Get(Asn.VAC));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


