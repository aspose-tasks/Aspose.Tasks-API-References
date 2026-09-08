---
title: "Filter.op_LessThanOrEqual"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Filter. Возвращает значение, указывающее, меньше ли этот экземпляр или равен указанному объекту"
type: docs
weight: 170
url: /ru/net/aspose.tasks/filter/op_lessthanorequal/
---
## Filter LessThanOrEqual operator

Возвращает значение, указывающее, меньше ли или равен этот экземпляр указанному объекту.

```csharp
public static bool operator <=(Filter a, Filter b)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| a | Filter | Первый фильтр. |
| b | Filter | Второй фильтр. |

### Возвращаемое значение

значение, указывающее, меньше ли этот экземпляр или равен указанному объекту

## Примеры

Показывает, как проверить равенство фильтров.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Filter> filters = project.TaskFilters.ToList();

var filter1 = filters[0];
var filter2 = filters[1];

// равенство фильтров проверяется по UID фильтра.
Console.WriteLine("Filter 1 UID: " + filter1.Uid);
Console.WriteLine("Filter 2 UID: " + filter2.Uid);
Console.WriteLine("Are filters equal: " + filter1.Equals(filter2));
```

### См. также

* class [Filter](../)
* namespace [Aspose.Tasks](../../filter/)
* assembly [Aspose.Tasks](../../../)


