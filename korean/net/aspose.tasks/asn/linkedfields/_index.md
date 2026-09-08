---
title: "Asn.LinkedFields"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Asn 필드. 프로젝트가 다른 OLE 개체와 연결되어 있는지 여부를 결정합니다"
type: docs
weight: 320
url: /ko/net/aspose.tasks/asn/linkedfields/
---
## Asn.LinkedFields field

프로젝트가 다른 OLE 개체와 연결되어 있는지 여부를 결정합니다.

```csharp
public static readonly Key<bool, AsnKey> LinkedFields;
```

## 예제

Asn.LinkedFields 속성을 읽는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine("Linked Fields: " + assignment.Get(Asn.LinkedFields));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


