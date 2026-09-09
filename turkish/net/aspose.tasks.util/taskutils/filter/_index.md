---
title: "TaskUtils.Filter"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "TaskUtils yöntemi. Koşulu sağlayan görevlerin yeni bir ağacını oluşturur"
type: docs
weight: 20
url: /tr/net/aspose.tasks.util/taskutils/filter/
---
## TaskUtils.Filter method

Koşulu sağlayan görevlerden yeni bir ağaç oluşturur.

```csharp
public static Task Filter(Task root, ICondition<Task> cond)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| root | Görev | Ağacın kökü. |
| cond | ICondition`1 | Uygulanan koşul. |

### Dönüş Değeri

Yeni bir ağacın kökü.

## Örnekler

Bir koşul ile nasıl çalışılacağını gösterir.

```csharp
[Test] //ExSkip
public void WorkWithFilter()
{
    var project = new Project(DataDir + "Project2.mpp");

    // Koşulu sağlayan görevlerin yeni bir ağacını oluşturur 
    var task = TaskUtils.Filter(project.RootTask, new FilterByDuration(2));

    // Bir ağaçtan görevleri toplar
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(task, coll, 0);

    // Düz bir görev listesi üzerinde yineleme yapar 
    // süreleri 2 iş gününden büyük veya eşit olan
    foreach (var collTask in coll.Tasks)
    {
        Console.WriteLine("Name: " + collTask.Get(Tsk.Name) + "Duration: " + collTask.Get(Tsk.Duration).TimeSpan);
    }
}

private class FilterByDuration : ICondition<Task>
{
    private readonly int days;

    public FilterByDuration(int days)
    {
        this.days = days;
    }

    /// <summary>
    /// Belirtilen nesne koşulları karşılıyorsa true döndürür.
    /// </summary>
    /// <param name=\"el\">Kontrol edilecek nesne.</param>
    /// <returns>Nesne koşulları karşılıyorsa true döndürür.</returns>
    /// <inheritdoc />
    public bool Check(Task el)
    {
        return el.Get(Tsk.Duration).TimeSpan >= TimeSpan.FromHours(this.days * 8);
    }
}
```

### Ayrıca Bakınız

* class [Task](../../../aspose.tasks/task/)
* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


