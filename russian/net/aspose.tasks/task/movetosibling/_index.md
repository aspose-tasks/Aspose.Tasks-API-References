---
title: "Task.MoveToSibling"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Task. Перемещает текущую задачу на том же Outline Level перед указанной задачей. Если ParentProject.CalculationMode равно None, пользователь должен вызвать Project.Recalculate после использования этого метода. Он перенесёт график всех задач проекта, установит даты начала/окончания, задаст ранние/поздние даты и вычислит зависимые поля, такие как slacks, work и cost fields, Outline levels. Если ParentProject.CalculationMode равно Manual, метод вычислит только task id, Outline level и Outline numbers автоматически. Если ParentProject.CalculationMode равно Automatic, метод автоматически перенесёт график всех задач проекта, установит даты начала/окончания, задаст ранние/поздние даты, вычислит slacks, work и cost fields, пересчитает ids и Outline levels."
type: docs
weight: 1370
url: /ru/net/aspose.tasks/task/movetosibling/
---
## MoveToSibling(Task) {#movetosibling}

Перемещает текущую задачу на том же уровне структуры перед указанной задачей. Если ParentProject.CalculationMode is None, пользователь должен вызвать Project.Recalculate() после использования этого метода (Это перенесёт все задачи проекта (даты начала/завершения, устанавливает ранние/поздние даты) и вычислит зависимые поля, такие как запасы времени, труд и стоимость, уровни структуры). Если ParentProject.CalculationMode is Manual метод вычислит только идентификатор задачи, уровень структуры и номера структуры автоматически. Если ParentProject.CalculationMode is Automatic метод перенесёт все задачи проекта автоматически (даты начала/завершения, устанавливает ранние/поздние даты, вычисляет запасы времени, труд и стоимость, пересчитывает идентификаторы и уровни структуры).

```csharp
public void MoveToSibling(Task beforeTask)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| beforeTask | Задача | Task, перед которой будет вставлена текущая задача. |

## Примеры

Показывает, как переместить задачу под тем же родителем.

```csharp
var project = new Project(DataDir + "MoveTask.mpp");

// Переместить задачи с id 5 перед задачей с id 3
var task = project.RootTask.Children.GetById(5);

var targetTask = project.RootTask.Children.First(t => t.Get(Tsk.Name) == "Task4");
task.MoveToSibling(targetTask);

// ИЛИ
// Переместить задачу в конец коллекции
// task.MoveToSibling(null);
project.Save(OutDir + "MoveTaskUnderSameParent_out.mpp", SaveFileFormat.Mpp);
```

### См. также

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)

---

## MoveToSibling(int) {#movetosibling_1}

Перемещает текущую задачу на том же уровне структуры перед задачей с указанным Id. Если ParentProject.CalculationMode is None, пользователь должен вызвать Project.Recalculate() после использования этого метода (Это перенесёт все задачи проекта (даты начала/завершения, устанавливает ранние/поздние даты) и вычислит зависимые поля, такие как запасы времени, труд и стоимость, уровни структуры). Если ParentProject.CalculationMode is Manual метод вычислит только идентификатор задачи, уровень структуры и номера структуры автоматически. Если ParentProject.CalculationMode is Automatic метод перенесёт все задачи проекта автоматически (даты начала/завершения, устанавливает ранние/поздние даты, вычисляет запасы времени, труд и стоимость, пересчитывает идентификаторы и уровни структуры).

```csharp
public void MoveToSibling(int beforeTaskId)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| beforeTaskId | Int32 | Id ([`Id`](../../tsk/id/)) задачи, перед которой будет вставлена текущая задача. |

## Примеры

Показывает, как переместить задачу под тем же родителем, используя Id задачи.

```csharp
var project = new Project(DataDir + "MoveTask.mpp");

// Переместить задачи с id 5 перед задачей с id 3
var task = project.RootTask.Children.GetById(5);

task.MoveToSibling(3);

// ИЛИ
// Переместить задачу в конец коллекции
// task.MoveToSibling(-1);
project.Save(OutDir + "MoveTaskUnderSameParent_out.mpp", SaveFileFormat.Mpp);
```

### См. также

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


