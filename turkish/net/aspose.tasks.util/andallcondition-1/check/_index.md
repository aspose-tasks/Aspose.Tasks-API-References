---
title: "AndAllCondition1.Check"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "AndAllCondition yöntemi. Belirtilen nesne koşulları sağlıyorsa true döndürür."
type: docs
weight: 20
url: /tr/net/aspose.tasks.util/andallcondition-1/check/
---
## AndAllCondition&lt;T&gt;.Check method

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

* class [AndAllCondition&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../andallcondition-1/)
* assembly [Aspose.Tasks](../../../)


