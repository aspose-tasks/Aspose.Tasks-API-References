---
title: "Project.SetBaseline"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Project. Сохраняет поля базовой линии в указанную базовую линию для всего проекта"
type: docs
weight: 1250
url: /ru/net/aspose.tasks/project/setbaseline/
---
## SetBaseline(BaselineType) {#setbaseline}

Сохраняет поля базового плана в указанный базовый план для всего проекта.

```csharp
public void SetBaseline(BaselineType baselineType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| baselineType | BaselineType | Тип базовой линии, в которую сохраняются данные базовой линии. |

## Примеры

Показывает, как создать базовые линии для всего проекта.

```csharp
var project = new Project();

// Добавление задач
project.RootTask.Children.Add("Task");
project.RootTask.Children.Add("Task2");

// Установить базовую линию для указанных задач
project.SetBaseline(BaselineType.Baseline);
```

### См. также

* enum [BaselineType](../../baselinetype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SetBaseline(BaselineType, IEnumerable&lt;Task&gt;) {#setbaseline_1}

Сохраняет поля базового плана в указанный базовый план для выбранных задач.

```csharp
public void SetBaseline(BaselineType baselineType, IEnumerable<Task> taskCollection)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| baselineType | BaselineType | Тип базовой линии, в которую сохраняются данные базовой линии. |
| taskCollection | IEnumerable`1 | Список задач, для которых сохраняются данные базовой линии. |

## Примеры

Показывает, как создать набор базовых линий для конкретных задач.

```csharp
var project = new Project();

// Добавление задач
var task = project.RootTask.Children.Add("Task");
var task2 = project.RootTask.Children.Add("Task2");

// Установить базовую линию для указанных задач
project.SetBaseline(BaselineType.Baseline, new[] { task, task2 });
```

### См. также

* enum [BaselineType](../../baselinetype/)
* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


