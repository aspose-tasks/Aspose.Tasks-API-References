---
title: "Asn.FixedMaterial"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Asn. Определяет, происходит ли потребление назначенного материального ресурса в виде единой фиксированной суммы"
type: docs
weight: 260
url: /ru/net/aspose.tasks/asn/fixedmaterial/
---
## Asn.FixedMaterial field

Определяет, происходит ли потребление назначенного материального ресурса в едином фиксированном объёме.

```csharp
public static readonly Key<bool, AsnKey> FixedMaterial;
```

## Примеры

Показывает, как читать/записывать свойство Asn.FixedMaterial.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.FixedMaterial, true);

Console.WriteLine("Fixed Material: " + assignment.Get(Asn.FixedMaterial));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


