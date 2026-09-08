---
title: "Asn.UpdateNeeded"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Asn 필드. 작업에 할당된 리소스가 작업 상태에 따라 업데이트가 필요한지 여부를 결정합니다"
type: docs
weight: 580
url: /ko/net/aspose.tasks/asn/updateneeded/
---
## Asn.UpdateNeeded field

작업에 할당된 리소스가 작업 상태에 따라 업데이트가 필요한지 여부를 결정합니다.

```csharp
public static readonly Key<bool, AsnKey> UpdateNeeded;
```

## 예제

Asn.UpdateNeeded 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.UpdateNeeded, true);

Console.WriteLine("Update Needed: " + assignment.Get(Asn.UpdateNeeded));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


