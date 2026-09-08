---
title: "Asn.UpdateNeeded"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Asn. Определяет, необходимо ли обновлять ресурс, назначенный задаче, в соответствии со статусом задачи."
type: docs
weight: 580
url: /ru/net/aspose.tasks/asn/updateneeded/
---
## Asn.UpdateNeeded field

Определяет, необходимо ли обновлять статус ресурса, назначенного задаче.

```csharp
public static readonly Key<bool, AsnKey> UpdateNeeded;
```

## Примеры

Показывает, как читать/записывать свойство Asn.UpdateNeeded.

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

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


