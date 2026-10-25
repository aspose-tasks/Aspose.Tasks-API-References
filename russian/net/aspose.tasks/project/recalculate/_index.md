---
title: "Project.Recalculate"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Project. Перепланирует все задачи проекта, их идентификаторы, уровни структуры, даты начала/завершения, устанавливает ранние/поздние даты, вычисляет запасы, рабочие и стоимостные поля"
type: docs
weight: 1150
url: /ru/net/aspose.tasks/project/recalculate/
---
## Recalculate() {#recalculate}

Перепланирует идентификаторы всех задач проекта, уровни структуры, даты начала/окончания, устанавливает ранние/поздние даты, вычисляет запасы времени, работу и поля стоимости.

```csharp
public void Recalculate()
```

## Примеры

Показывает, как перенести график проекта, начиная с даты начала, а не с даты завершения.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.ScheduleFromStart, true);
project.Set(Prj.StartDate, new DateTime(2014, 1, 1));

// Теперь рассчитываются все даты задач (Start, Finish, EarlyStart, EarlyFinish, LateStart, LateFinish). Чтобы получить критический путь, необходимо вычислить запасы (можно вызвать в отдельном потоке, но только после расчёта всех ранних/поздних дат).
project.Recalculate();

foreach (var task in project.CriticalPath)
{
    Console.WriteLine(task.Get(Tsk.Id));
    Console.WriteLine(task.Get(Tsk.Name));
}
```

### См. также

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Recalculate(bool) {#recalculate_1}

Перепланирует идентификаторы всех задач проекта, уровни структуры, даты начала/окончания, устанавливает ранние/поздние даты, вычисляет запасы времени, работу и поля стоимости с необязательной проверкой.

```csharp
public void Recalculate(bool validate)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| validate | Boolean | Если значение true, будет выполнена проверка пересчёта. Какие данные проверяются: в данный момент реализована только базовая проверка диапазонов дат задач и связей задач. Диапазоны дат задач (например, ActualStart - ActualFinish, EarlyStart - EarlyFinish и т.д.), а также даты связей задач будут проверяться на соответствие критерию, что дата начала меньше или равна дате завершения. Если любое из описанных выше условий не выполнено, будет выброшено исключение [`RecalculationValidationException`](../../recalculationvalidationexception/). |

## Примеры

Показывает, как пересчитать проект с последующей проверкой.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("t1");
task.Set(Tsk.CommitmentStart, new DateTime(2017, 6, 19, 8, 0, 0));
task.Set(Tsk.CommitmentFinish, new DateTime(2017, 6, 18, 17, 0, 0));

try
{
    // пересчитать проект с последующей проверкой
    project.Recalculate(true);
}
catch (TaskValidationException ex)
{
    Console.WriteLine(ex.Message);
}
```

### См. также

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


