---
title: "Класс AndAllConditionT"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Util.AndAllCondition1T. Применяет логическое И ко всем условиям. Например, cond1 AND cond2 AND cond3"
type: docs
weight: 2660
url: /ru/net/aspose.tasks.util/andallcondition-1/
---
## AndAllCondition&lt;T&gt; class

Применяет логическое И ко всем условиям. Например: cond1 AND cond2 AND cond3...

```csharp
public class AndAllCondition<T> : ICondition<T>
```

| Параметр | Описание |
| --- | --- |
| T | Тип объекта, к которому применяется интерфейс метода. |

## Конструкторы

| Имя | Описание |
| --- | --- |
| [AndAllCondition](andallcondition/)(List&lt;ICondition&lt;T&gt;&gt;) | Инициализирует новый экземпляр класса `AndAllCondition`. |

## Методы

| Имя | Описание |
| --- | --- |
| [Check](../../aspose.tasks.util/andallcondition-1/check/)(T) | Возвращает true, если указанный объект удовлетворяет условиям. |

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

* interface [ICondition&lt;T&gt;](../icondition-1/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


