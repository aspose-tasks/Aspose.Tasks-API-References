---
title: "TaskUtils.Find"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "TaskUtils yöntemi. Bir görev ağacındaki koşulu sağlayan bir görevi bulur."
type: docs
weight: 30
url: /tr/net/aspose.tasks.util/taskutils/find/
---
## TaskUtils.Find method

Görev ağacında koşulu sağlayan bir görevi bulur.

```csharp
public static Task Find(Task root, ICondition<Task> cond)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| root | Görev | Ağacın kökü. |
| cond | ICondition`1 | Uygulanan koşul. |

### Dönüş Değeri

Task, görev bulunmuşsa, aksi takdirde null.

## Örnekler

&lt;see cref="Aspose.Tasks.Util.TaskUtils.Find" /&gt; yönteminin nasıl kullanılacağını gösterir.

```csharp
public void WorkWithFind()
{
    var project = new Project(DataDir + "Project2.mpp");

    // Koşulu sağlayan görevlerin yeni bir ağacını oluşturur 
    var task = TaskUtils.Filter(project.RootTask, new FindByName("Task8"));

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

private class FindByName : ICondition<Task>
{
    private readonly string name;

    public FindByName(string name)
    {
        this.name = name;
    }

    /// <summary>
    /// Belirtilen nesne koşulları karşılıyorsa true döndürür.
    /// </summary>
    /// <param name=\"el\">Kontrol edilecek nesne.</param>
    /// <returns>Nesne koşulları karşılıyorsa true döndürür.</returns>
    /// <inheritdoc />
    public bool Check(Task el)
    {
        return el.Get(Tsk.Name) == this.name;
    }
}
```

### Ayrıca Bakınız

* class [Task](../../../aspose.tasks/task/)
* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


