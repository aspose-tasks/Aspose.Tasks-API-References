---
title: "Asn.Created"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Asn 필드. 할당이 생성된 날짜"
type: docs
weight: 210
url: /ko/net/aspose.tasks/asn/created/
---
## Asn.Created field

과제가 생성된 날짜.

```csharp
public static readonly Key<DateTime, AsnKey> Created;
```

## 예제

Asn.Created 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Created, new DateTime(2020, 4, 9, 8, 0, 0));

Console.WriteLine("Created: " + assignment.Get(Asn.Created));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


