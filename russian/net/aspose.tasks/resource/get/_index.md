---
title: "Resource.Get"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Resource. Возвращает значение, к которому свойство сопоставлено в этом контейнере"
type: docs
weight: 830
url: /ru/net/aspose.tasks/resource/get/
---
## Resource.Get&lt;T&gt; method

Возвращает значение, к которому свойство сопоставлено в этом контейнере.

```csharp
public T Get<T>(Key<T, RscKey> key)
```

| Параметр | Описание |
| --- | --- |
| T | тип сопоставленного значения. |
| key | указанный ключ свойства. [`Rsc`](../../rsc/) для получения ключа свойства. |

### Возвращаемое значение

значение, к которому свойство сопоставлено в этом контейнере.

## Примеры

Показывает, как читать/записывать общие свойства ресурса.

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
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


