---
title: "Asn.RegularWork"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Asn. Объём работы без сверхурочных, запланированной для назначения"
type: docs
weight: 420
url: /ru/net/aspose.tasks/asn/regularwork/
---
## Asn.RegularWork field

Объём работы без сверхурочных, запланированной для назначения.

```csharp
public static readonly Key<Duration, AsnKey> RegularWork;
```

## Примеры

Показывает, как читать/записывать свойство Asn.RegularWork.

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

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


