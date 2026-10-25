---
title: "Not1.Not"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Not yapıcı. Not sınıfının yeni bir örneğini başlatır."
type: docs
weight: 10
url: /tr/net/aspose.tasks.util/not-1/not/
---
## Not&lt;T&gt; constructor

Yeni bir [`Not`](../) sınıf örneğini başlatır.

```csharp
public Not(ICondition<T> condition)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| koşul | ICondition`1 | Belirtilen koşul. |

## Örnekler

Nasıl &lt;see cref=\"Aspose.Tasks.Util.Not`1\" /&gt; koşulunun kullanılacağını gösterir.

```csharp
public void WorkWithNot()
{
    var project = new Project(DataDir + "Project2.mpp");

    // tüm proje görevlerini topla
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, coll, 0);

    // bir filtre koşulu oluştur
    var filter = new NullCondition();

    // ve <see cref=\"Aspose.Tasks.Util.Not`1\" /> koşulunu uygulayarak tersine çevir
    var condition = new Not<Task>(filter);

    // koşulu toplanan görevlere uygula
    List<Task> collection = Filter(coll.Tasks, condition);
    foreach (var task in collection)
    {
        Console.WriteLine("Name: " + task.Get(Tsk.Name));

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

private class NullCondition : ICondition<Task>
{
    public bool Check(Task el)
    {
        return el.Get(Tsk.IsNull).Value;
    }
}
```

### Ayrıca Bakınız

* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [Not&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../not-1/)
* assembly [Aspose.Tasks](../../../)


