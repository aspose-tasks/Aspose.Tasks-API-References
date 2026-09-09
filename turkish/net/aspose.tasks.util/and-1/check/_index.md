---
title: "And1.Check"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "And yöntemi. Belirtilen nesne koşulları sağlarsa doğru döndürür"
type: docs
weight: 20
url: /tr/net/aspose.tasks.util/and-1/check/
---
## And&lt;T&gt;.Check method

Belirtilen nesne koşulları sağlarsa true döndürür.

```csharp
public bool Check(T el)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| el | T | Kontrol edilecek nesne. |

### Dönüş Değeri

Nesne koşulları sağlarsa doğru.

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

* class [And&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../and-1/)
* assembly [Aspose.Tasks](../../../)


