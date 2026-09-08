---
title: "Asn.RegularWork"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Asn 필드. 할당에 대해 예정된 비초과 근무량"
type: docs
weight: 420
url: /ko/net/aspose.tasks/asn/regularwork/
---
## Asn.RegularWork field

할당에 대해 예정된 비초과 근무 작업량.

```csharp
public static readonly Key<Duration, AsnKey> RegularWork;
```

## 예제

Asn.RegularWork 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.RegularWork, project.GetWork(1));

Console.WriteLine("Regular Work: " + assignment.Get(Asn.RegularWork));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


