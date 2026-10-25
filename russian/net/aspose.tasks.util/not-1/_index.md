---
title: "Класс NotT"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Util.Not1T. Применяет логическое NOT к указанному условию"
type: docs
weight: 2750
url: /ru/net/aspose.tasks.util/not-1/
---
## Not&lt;T&gt; class

Применяет логическое НЕ к указанному условию.

```csharp
public class Not<T> : ICondition<T>
```

| Параметр | Описание |
| --- | --- |
| T | Тип объекта, к которому применяется интерфейс метода. |

## Конструкторы

| Имя | Описание |
| --- | --- |
| [Not](not/)(ICondition&lt;T&gt;) | Инициализирует новый экземпляр класса `Not`. |

## Методы

| Имя | Описание |
| --- | --- |
| [Check](../../aspose.tasks.util/not-1/check/)(T) | Возвращает true, если указанный объект удовлетворяет условию. |

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

* interface [ICondition&lt;T&gt;](../icondition-1/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


