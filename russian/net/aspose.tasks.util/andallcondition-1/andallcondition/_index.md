---
title: "AndAllCondition1.AndAllCondition"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конструктор AndAllCondition. Инициализирует новый экземпляр класса AndAllCondition"
type: docs
weight: 10
url: /ru/net/aspose.tasks.util/andallcondition-1/andallcondition/
---
## AndAllCondition&lt;T&gt; constructor

Инициализирует новый экземпляр класса [`AndAllCondition`](../).

```csharp
public AndAllCondition(List<ICondition<T>> conditions)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| условия | List`1 | Список условий. |

## Примеры

Показывает, как использовать условие &lt;see cref="Aspose.Tasks.Util.AndAllCondition`1" /&gt;.

```csharp
public void WorkWithAndAllCondition()
{
    var project = new Project(DataDir + "Project2.mpp");

    // собрать все задачи проекта
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, coll, 0);

    var conditions = new List<ICondition<Task>>
                         {
                             // создать условие фильтра, которое отбирает задачи, не равные null
                             new NotNullCondition(),

                             // создать условие фильтра, которое отбирает сводные задачи
                             new SummaryCondition()
                         };

    // и объедините их, применяя условие <see cref="Aspose.Tasks.Util.AndAllCondition`1" />
    var joinedCondition = new AndAllCondition<Task>(conditions);

    // применить условие к собранным задачам
    List<Task> collection = Filter(coll.Tasks, joinedCondition);
    Console.WriteLine("Filtered tasks: ");
    foreach (var task in collection)
    {
        Console.WriteLine("  Name: " + task.Get(Tsk.Name));

        // работать с другими свойствами...
    }

    // ...
}

private static List<T> Filter<T>(IEnumerable<T> array, ICondition<T> cond)
{
    var result = new List<T>();

    foreach (var item in array)
    {
        if (cond.Check(item))
        {
            result.Add(item);
        }
    }

    return result;
}

private class NotNullCondition : ICondition<Task>
{
    public bool Check(Task el)
    {
        return !el.Get(Tsk.IsNull).Value;
    }
}

private class SummaryCondition : ICondition<Task>
{
    public bool Check(Task el)
    {
        return el.Get(Tsk.IsSummary);
    }
}
```

### См. также

* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [AndAllCondition&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../andallcondition-1/)
* assembly [Aspose.Tasks](../../../)


