---
title: "Sınıf AndAllConditionT"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Util.AndAllCondition1T sınıfı. Tüm koşullara mantıksal AND uygular. Örneğin cond1 AND cond2 AND cond3"
type: docs
weight: 2660
url: /tr/net/aspose.tasks.util/andallcondition-1/
---
## AndAllCondition&lt;T&gt; class

Tüm koşullara mantıksal VE uygular. Örneğin: cond1 AND cond2 AND cond3...

```csharp
public class AndAllCondition<T> : ICondition<T>
```

| Parametre | Açıklama |
| --- | --- |
| T | Yöntem arayüzünün uygulanacağı nesnenin türü. |

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [AndAllCondition](andallcondition/)(List&lt;ICondition&lt;T&gt;&gt;) | `AndAllCondition` sınıfının yeni bir örneğini başlatır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Check](../../aspose.tasks.util/andallcondition-1/check/)(T) | Belirtilen nesne koşulları sağlarsa true döndürür. |

## Örnekler

&lt;see cref=\"Aspose.Tasks.Util.AndAllCondition`1\" /&gt; koşulunun nasıl kullanılacağını gösterir.

```csharp
public void WorkWithAndAllCondition()
{
    var project = new Project(DataDir + "Project2.mpp");

    // tüm proje görevlerini topla
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, coll, 0);

    var conditions = new List<ICondition<Task>>
                         {
                             // null olmayan görevleri filtreleyen bir filtre koşulu oluştur
                             new NotNullCondition(),

                             // özet görevleri filtreleyen bir filtre koşulu oluştur
                             new SummaryCondition()
                         };

    // ve <see cref=\"Aspose.Tasks.Util.AndAllCondition`1\" /> koşulunu uygulayarak onları birleştir
    var joinedCondition = new AndAllCondition<Task>(conditions);

    // koşulu toplanan görevlere uygula
    List<Task> collection = Filter(coll.Tasks, joinedCondition);
    Console.WriteLine("Filtered tasks: ");
    foreach (var task in collection)
    {
        Console.WriteLine("  Name: " + task.Get(Tsk.Name));

        // diğer özelliklerle çalış...
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

### Ayrıca Bakınız

* interface [ICondition&lt;T&gt;](../icondition-1/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


