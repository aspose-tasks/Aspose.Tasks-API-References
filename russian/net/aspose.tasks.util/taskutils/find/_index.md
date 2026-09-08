---
title: "TaskUtils.Find"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод TaskUtils. Находит задачу, которая удовлетворяет условию в дереве задач"
type: docs
weight: 30
url: /ru/net/aspose.tasks.util/taskutils/find/
---
## TaskUtils.Find method

Находит задачу, удовлетворяющую условию, в дереве задач.

```csharp
public static Task Find(Task root, ICondition<Task> cond)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| root | Задача | Корень дерева. |
| cond | ICondition`1 | Применённое условие. |

### Возвращаемое значение

Task, если задача найдена, иначе null.

## Примеры

Показывает, как использовать &lt;see cref=\"Aspose.Tasks.Util.TaskUtils.Find\" /&gt; метод.

```csharp
public void WorkWithFind()
{
    var project = new Project(DataDir + "Project2.mpp");

    // создаёт новое дерево задач, удовлетворяющих условию 
    var task = TaskUtils.Filter(project.RootTask, new FindByName("Task8"));

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

private class FindByName : ICondition<Task>
{
    private readonly string name;

    public FindByName(string name)
    {
        this.name = name;
    }

    /// <summary>
    /// Возвращает true, если указанный объект удовлетворяет условиям.
    /// </summary>
    /// <param name="el">Объект для проверки.</param>
    /// <returns>True, если объект удовлетворяет условиям.</returns>
    /// <inheritdoc />
    public bool Check(Task el)
    {
        return el.Get(Tsk.Name) == this.name;
    }
}
```

### См. также

* class [Task](../../../aspose.tasks/task/)
* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


