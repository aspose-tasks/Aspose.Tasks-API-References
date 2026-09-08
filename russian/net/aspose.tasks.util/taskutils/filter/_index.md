---
title: "TaskUtils.Filter"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод TaskUtils. Создаёт новое дерево задач, удовлетворяющих условию"
type: docs
weight: 20
url: /ru/net/aspose.tasks.util/taskutils/filter/
---
## TaskUtils.Filter method

Создаёт новое дерево задач, удовлетворяющих условию.

```csharp
public static Task Filter(Task root, ICondition<Task> cond)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| root | Задача | Корень дерева. |
| cond | ICondition`1 | Применённое условие. |

### Возвращаемое значение

Корень нового дерева.

## Примеры

Показывает, как работать с условием.

```csharp
[Test] //ExSkip
public void WorkWithFilter()
{
    var project = new Project(DataDir + "Project2.mpp");

    // создаёт новое дерево задач, удовлетворяющих условию 
    var task = TaskUtils.Filter(project.RootTask, new FilterByDuration(2));

    // собрать задачи из дерева
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(task, coll, 0);

    // перебрать простой список задач 
    // у которых длительность больше или равна 2 рабочим дням
    foreach (var collTask in coll.Tasks)
    {
        Console.WriteLine("Name: " + collTask.Get(Tsk.Name) + "Duration: " + collTask.Get(Tsk.Duration).TimeSpan);
    }
}

private class FilterByDuration : ICondition<Task>
{
    private readonly int days;

    public FilterByDuration(int days)
    {
        this.days = days;
    }

    /// <summary>
    /// Возвращает true, если указанный объект удовлетворяет условиям.
    /// </summary>
    /// <param name="el">Объект для проверки.</param>
    /// <returns>True, если объект удовлетворяет условиям.</returns>
    /// <inheritdoc />
    public bool Check(Task el)
    {
        return el.Get(Tsk.Duration).TimeSpan >= TimeSpan.FromHours(this.days * 8);
    }
}
```

### См. также

* class [Task](../../../aspose.tasks/task/)
* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


