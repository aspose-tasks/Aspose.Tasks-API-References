---
title: "Rsc.Group"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Группа, к которой принадлежит ресурс"
type: docs
weight: 300
url: /ru/net/aspose.tasks/rsc/group/
---
## Rsc.Group field

Группа, к которой относится ресурс.

```csharp
public static readonly Key<string, RscKey> Group;
```

## Примеры

Показывает, как работать с тарифами ресурсов и группами.

```csharp
var project = new Project(DataDir + "UpdateResourceData.mpp");

// Добавить ресурс и установить некоторые свойства
var resource = project.Resources.Add("Rsc");
resource.Set(Rsc.Start, new DateTime(2020, 4, 1, 8, 0, 0));
resource.Set(Rsc.StandardRate, 30);
resource.Set(Rsc.OvertimeRate, 45);
resource.Set(Rsc.Group, "Workgroup1");

Console.WriteLine("Resource Start: " + resource.Get(Rsc.Start));
Console.WriteLine("Resource Standard Rate: " + resource.Get(Rsc.StandardRate));
Console.WriteLine("Resource Overtime Rate: " + resource.Get(Rsc.OvertimeRate));
Console.WriteLine("Resource Group: " + resource.Get(Rsc.Group));

project.Save(OutDir + "UpdateResourceData_out.mpp", SaveFileFormat.Mpp);
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


