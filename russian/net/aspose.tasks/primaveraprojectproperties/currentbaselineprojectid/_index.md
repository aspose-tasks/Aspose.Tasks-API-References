---
title: "PrimaveraProjectProperties.CurrentBaselineProjectId"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство PrimaveraProjectProperties. Возвращает идентификатор текущего базового проекта. Применимо к проектам, читаемым из Primavera XML файлов, содержащих экспортированные базовые линии"
type: docs
weight: 40
url: /ru/net/aspose.tasks/primaveraprojectproperties/currentbaselineprojectid/
---
## PrimaveraProjectProperties.CurrentBaselineProjectId property

Получает идентификатор текущего базового проекта. Применимо к проектам, прочитанным из XML‑файлов Primavera, содержащих экспортированные базовые версии.

```csharp
public int CurrentBaselineProjectId { get; }
```

## Примеры

Показывает, как прочитать проект из файла Primavera XML и изучить данные базовых проектов.

```csharp
Project project = new Project(DataDir + "BaselineProjects.xml");

Console.WriteLine("Current baseline project uid: " + project.PrimaveraProperties.CurrentBaselineProjectId);

foreach (var baselineProject in project.PrimaveraProperties.BaselineProjects)
{
    Console.WriteLine("Baseline project: uid: {0}, name: '{1}'", baselineProject.Uid, baselineProject.Name);
}

var baseline1 = project.PrimaveraProperties.BaselineProjects[1];

var task = GetTaskByActivityId(project, "A1000");
var baselineTask = GetTaskByActivityId(baseline1, "A1000");

Console.WriteLine("Task budgeted total cost: " + task.PrimaveraProperties.BudgetedTotalCost);
Console.WriteLine("Task baseline budgeted total cost: " + baselineTask.PrimaveraProperties.BudgetedTotalCost);
```

### См. также

* class [PrimaveraProjectProperties](../)
* namespace [Aspose.Tasks](../../primaveraprojectproperties/)
* assembly [Aspose.Tasks](../../../)


