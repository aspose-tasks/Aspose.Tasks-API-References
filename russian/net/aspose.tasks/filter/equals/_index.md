---
title: "Filter.Equals"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Filter. Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту AssignmentBaseline"
type: docs
weight: 100
url: /ru/net/aspose.tasks/filter/equals/
---
## Equals(Filter) {#equals}

Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту AssignmentBaseline.

```csharp
public bool Equals(Filter other)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| другой | Filter | указанный объект AssignmentBaseline для сравнения с этим экземпляром. |

### Возвращаемое значение

возвращает true, если этот экземпляр равен указанному объекту AssignmentBaseline; в противном случае — false.

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

---

## Equals(object) {#equals_1}

Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту AssignmentBaseline.

```csharp
public override bool Equals(object obj)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| obj | Объект | указанный объект AssignmentBaseline для сравнения с этим экземпляром. |

### Возвращаемое значение

возвращает true, если этот экземпляр равен указанному объекту AssignmentBaseline; в противном случае — false.

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


