---
title: "Класс AndT"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Util.And1T. Применяет логическое И к указанным условиям"
type: docs
weight: 2670
url: /ru/net/aspose.tasks.util/and-1/
---
## And&lt;T&gt; class

Применяет логическое И к указанным условиям.

```csharp
public class And<T> : ICondition<T>
```

| Параметр | Описание |
| --- | --- |
| T | Тип объекта, к которому применяется интерфейс метода. |

## Конструкторы

| Имя | Описание |
| --- | --- |
| [And](and/)(ICondition&lt;T&gt;, ICondition&lt;T&gt;) | Инициализирует новый экземпляр класса `And`. |

## Методы

| Имя | Описание |
| --- | --- |
| [Check](../../aspose.tasks.util/and-1/check/)(T) | Возвращает true, если указанный объект удовлетворяет условиям. |

## Примеры

Показывает, как использовать условие &lt;see cref=\"Aspose.Tasks.Util.And`1\" /&gt;.

```csharp
public void WorkWithAnd()
{
    var project = new Project(DataDir + "Project2.mpp");

    // собрать все задачи проекта
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, coll, 0);

    // создать условие фильтра, которое отбирает сводные задачи
    var condition1 = new SummaryCondition();

    // создать условие фильтра, которое отбирает задачи, не равные null
    var condition2 = new NotNullCondition();

    // и объединить их, применив условие <see cref=\"Aspose.Tasks.Util.And`1\" />
    var joinedCondition = new And<Task>(condition1, condition2);

    // применить условие к собранным задачам
    List<Task> collection = Filter(coll.Tasks, joinedCondition);
    Console.WriteLine("Filtered tasks: ");
    foreach (var task in collection)
    {
        Console.WriteLine(" Name: " + task.Get(Tsk.Name));

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


