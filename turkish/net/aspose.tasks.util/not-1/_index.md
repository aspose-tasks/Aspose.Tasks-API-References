---
title: "Sınıf NotT"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Util.Not1T sınıfı. Belirtilen koşula mantıksal NOT uygular"
type: docs
weight: 2750
url: /tr/net/aspose.tasks.util/not-1/
---
## Not&lt;T&gt; class

Belirtilen koşula mantıksal DEĞİL uygular.

```csharp
public class Not<T> : ICondition<T>
```

| Parametre | Açıklama |
| --- | --- |
| T | Yöntem arayüzünün uygulanacağı nesnenin türü. |

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [Not](not/)(ICondition&lt;T&gt;) | `Not` sınıfının yeni bir örneğini başlatır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Check](../../aspose.tasks.util/not-1/check/)(T) | Belirtilen nesne koşulu sağlarsa true döndürür. |

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

* interface [ICondition&lt;T&gt;](../icondition-1/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


