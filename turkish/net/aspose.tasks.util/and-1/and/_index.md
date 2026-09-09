---
title: "And1.And"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "And yapıcı. And sınıfının yeni bir örneğini başlatır"
type: docs
weight: 10
url: /tr/net/aspose.tasks.util/and-1/and/
---
## And&lt;T&gt; constructor

[`And`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public And(ICondition<T> cond1, ICondition<T> cond2)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cond1 | ICondition`1 | İlk koşul. |
| cond2 | ICondition`1 | İkinci koşul. |

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

* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [And&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../and-1/)
* assembly [Aspose.Tasks](../../../)


