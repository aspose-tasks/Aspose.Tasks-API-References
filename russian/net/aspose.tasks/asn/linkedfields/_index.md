---
title: "Asn.LinkedFields"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Asn. Определяет, связан ли проект с другим объектом OLE"
type: docs
weight: 320
url: /ru/net/aspose.tasks/asn/linkedfields/
---
## Asn.LinkedFields field

Определяет, связан ли проект с другим объектом OLE.

```csharp
public static readonly Key<bool, AsnKey> LinkedFields;
```

## Примеры

Показывает, как читать свойство Asn.LinkedFields.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine("Linked Fields: " + assignment.Get(Asn.LinkedFields));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


