---
title: "ResourceAssignment.SetMaterialResourceUnits"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод ResourceAssignment. Устанавливает единицы для назначения материального ресурса с переменным потреблением материалов. Переменное потребление материалов означает, что при изменении длительности назначения количество используемых материалов меняется пропорционально"
type: docs
weight: 760
url: /ru/net/aspose.tasks/resourceassignment/setmaterialresourceunits/
---
## ResourceAssignment.SetMaterialResourceUnits method

Устанавливает единицы измерения для назначения материального ресурса с переменным потреблением материалов. Переменное потребление материалов означает, что при изменении длительности назначения количество используемых материалов меняется пропорционально.

```csharp
public void SetMaterialResourceUnits(double units, RateScaleType rateScaleType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| единицы | Double | Количество единиц, начисленных за период времени. |
| rateScaleType | RateScaleType | Период времени, в который начисляется значение единицы. |

### Исключения

| исключение | условие |
| --- | --- |
| InvalidOperationException | Если метод вызывается для назначения нематериального ресурса. |

## Примечания

Например, чтобы установить '123/мес', следует вызвать SetUnitsScaled(123D, RateScaleType.Month).

## Примеры

Показывает, как установить переменное потребление материалов (например, '10/day' или '1/week') для назначения материального ресурса.

```csharp
var project = new Project(DataDir + "New project 2013.mpp");

var task = project.RootTask.Children.Add("t1");

var materialResource = project.Resources.Add("materialResource");
materialResource.Set(Rsc.Type, ResourceType.Material);

var materialResourceAssignment = project.ResourceAssignments.Add(task, materialResource);

// Предположим, что мы хотим установить потребление материалов '1/week'.
materialResourceAssignment.SetMaterialResourceUnits(1D, RateScaleType.Week);
```

### См. также

* enum [RateScaleType](../../ratescaletype/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


