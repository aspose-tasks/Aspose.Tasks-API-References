---
title: "Перечисление RateScaleType"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.RateScaleType. Указывает тип шкалы ставки"
type: docs
weight: 1650
url: /ru/net/aspose.tasks/ratescaletype/
---
## RateScaleType enumeration

Указывает тип шкалы ставки.

```csharp
public enum RateScaleType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Undefined | `0` | Указывает тип шкалы ставки Undefined. |
| Minute | `1` | Указывает тип шкалы ставки Minute. |
| Hour | `2` | Указывает тип шкалы ставки Hour. |
| Day | `3` | Указывает тип шкалы ставки Day. |
| Week | `4` | Указывает тип шкалы ставки Week. |
| Month | `5` | Указывает тип шкалы ставки Month. |
| Quarter | `6` | Указывает тип шкалы ставки Quarter. |
| Year | `7` | Указывает тип шкалы ставки Year. |

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

Показывает, как работать с шкалой ставки назначения, когда мы хотим установить переменное потребление материалов (например, '10/day' или '1/week') для назначения материального ресурса.

```csharp
var project = new Project(DataDir + "New project 2013.mpp");

var task = project.RootTask.Children.Add("t1");

var materialResource = project.Resources.Add("materialResource");
materialResource.Set(Rsc.Type, ResourceType.Material);

var nonMaterialResource = project.Resources.Add("nonMaterialResource");
nonMaterialResource.Set(Rsc.Type, ResourceType.Work);

var materialResourceAssignment = project.ResourceAssignments.Add(task, materialResource);

// Предположим, что мы хотим установить потребление материалов '1/week'.
// Нужно установить почасовую ставку в свойство Units, поэтому мы делим 1D на часы в неделе.
materialResourceAssignment.Set(Asn.Units, 1D / 40);
materialResourceAssignment.Set(Asn.RateScale, RateScaleType.Week);

// Обратите внимание, что начиная с версии 24.4 это можно сделать, вызвав один метод:
// materialResourceAssignment.SetMaterialResourceUnits(1D, RateScaleType.Week);

var nonMaterialResourceAssignment = project.ResourceAssignments.Add(task, nonMaterialResource);
nonMaterialResourceAssignment.Set(Asn.RateScale, RateScaleType.Week);

project.Save(OutDir + "ReadWriteRateScaleForResourceAssignment_out.mpp", SaveFileFormat.Mpp);

var resavedProject = new Project(OutDir + "ReadWriteRateScaleForResourceAssignment_out.mpp");

var resavedMaterialResourceAssignment = resavedProject.ResourceAssignments.GetByUid(2);
Console.WriteLine(resavedMaterialResourceAssignment.Get(Asn.RateScale));

// Только назначения материальных ресурсов могут иметь ненулевое значение шкалы ставки.
var resavedNonMaterialResourceAssignment = resavedProject.ResourceAssignments.GetByUid(3);
Console.WriteLine(resavedNonMaterialResourceAssignment.Get(Asn.RateScale));
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


