---
title: "Not1.Check"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Not. Возвращает true, если указанный объект удовлетворяет условию."
type: docs
weight: 20
url: /ru/net/aspose.tasks.util/not-1/check/
---
## Not&lt;T&gt;.Check method

Возвращает true, если указанный объект удовлетворяет условию.

```csharp
public bool Check(T el)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| el | T | Объект для проверки. |

### Возвращаемое значение

True, если объект удовлетворяет условию.

## Примеры

Показывает, как использовать условие &lt;see cref=\"Aspose.Tasks.Util.Not`1\" /&gt;.

```csharp
public void WorkWithNot()
{
    var project = new Project(DataDir + "Project2.mpp");

    // собрать все задачи проекта
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, coll, 0);

    // создать условие фильтра
    var filter = new NullCondition();

    // и обратить его, применив условие <see cref=\"Aspose.Tasks.Util.Not`1\" />
    var condition = new Not<Task>(filter);

    // применить условие к собранным задачам
    List<Task> collection = Filter(coll.Tasks, condition);
    foreach (var task in collection)
    {
        Console.WriteLine("Name: " + task.Get(Tsk.Name));

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

private class NullCondition : ICondition<Task>
{
    public bool Check(Task el)
    {
        return el.Get(Tsk.IsNull).Value;
    }
}
```

### См. также

* class [Not&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../not-1/)
* assembly [Aspose.Tasks](../../../)


