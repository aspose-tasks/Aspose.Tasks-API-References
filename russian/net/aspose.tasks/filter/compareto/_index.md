---
title: "Filter.CompareTo"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Filter. Сравнивает этот экземпляр с указанным экземпляром класса Filter и возвращает указание их относительного порядка"
type: docs
weight: 90
url: /ru/net/aspose.tasks/filter/compareto/
---
## Filter.CompareTo method

Сравнивает этот экземпляр с указанным экземпляром класса [`Filter`](../) и возвращает указание их относительного порядка.

```csharp
public int CompareTo(Filter other)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| other | Filter | указанный экземпляр класса [`Filter`](../) для сравнения с этим объектом. |

### Возвращаемое значение

указание их относительного порядка.

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


