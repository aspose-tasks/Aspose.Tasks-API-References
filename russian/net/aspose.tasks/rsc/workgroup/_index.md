---
title: "Rsc.Workgroup"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Тип рабочей группы, к которой принадлежит ресурс"
type: docs
weight: 700
url: /ru/net/aspose.tasks/rsc/workgroup/
---
## Rsc.Workgroup field

Тип рабочей группы, к которой принадлежит ресурс.

```csharp
public static readonly Key<WorkGroupType, RscKey> Workgroup;
```

## Примеры

Показывает, как читать/записывать свойство Rsc.Workgroup.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Workgroup, WorkGroupType.Email);

Console.WriteLine("Workgroup: " + resource.Get(Rsc.Workgroup));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [WorkGroupType](../../workgrouptype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


