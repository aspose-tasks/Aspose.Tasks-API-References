---
title: "Sınıf AndT"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Util.And1T sınıfı. Belirtilen koşullara mantıksal AND uygular"
type: docs
weight: 2670
url: /tr/net/aspose.tasks.util/and-1/
---
## And&lt;T&gt; class

Belirtilen koşullara mantıksal VE uygular.

```csharp
public class And<T> : ICondition<T>
```

| Parametre | Açıklama |
| --- | --- |
| T | Yöntem arayüzünün uygulanacağı nesnenin türü. |

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [And](and/)(ICondition&lt;T&gt;, ICondition&lt;T&gt;) | `And` sınıfının yeni bir örneğini başlatır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Check](../../aspose.tasks.util/and-1/check/)(T) | Belirtilen nesne koşulları sağlarsa true döndürür. |

## Örnekler

Nasıl &lt;see cref=\"Aspose.Tasks.Util.And`1\" /&gt; koşulunun kullanılacağını gösterir.

```csharp
public void WorkWithAnd()
{
    var project = new Project(DataDir + "Project2.mpp");

    // tüm proje görevlerini topla
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, coll, 0);

    // özet görevleri filtreleyen bir filtre koşulu oluştur
    var condition1 = new SummaryCondition();

    // null olmayan görevleri filtreleyen bir filtre koşulu oluştur
    var condition2 = new NotNullCondition();

    // ve <see cref=\"Aspose.Tasks.Util.And`1\" /> koşulunu uygulayarak birleştir
    var joinedCondition = new And<Task>(condition1, condition2);

    // koşulu toplanan görevlere uygula
    List<Task> collection = Filter(coll.Tasks, joinedCondition);
    Console.WriteLine("Filtered tasks: ");
    foreach (var task in collection)
    {
        Console.WriteLine(" Name: " + task.Get(Tsk.Name));

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


