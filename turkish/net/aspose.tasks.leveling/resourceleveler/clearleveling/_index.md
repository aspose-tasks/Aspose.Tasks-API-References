---
title: "ResourceLeveler.ClearLeveling"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ResourceLeveler yöntemi. Kaynak dengelemesi sırasında projeye daha önce eklenmiş herhangi bir dengeleme gecikmesini temizler."
type: docs
weight: 10
url: /tr/net/aspose.tasks.leveling/resourceleveler/clearleveling/
---
## ClearLeveling(Project) {#clearleveling}

Kaynak dengelemesi sırasında projeye daha önce eklenmiş olan herhangi bir dengeleme gecikmesini temizler.

```csharp
public static void ClearLeveling(Project project)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| project | Project | Dengelemeyi temizleyecek proje. |

## Örnekler

Varsayılan seçenekleri kullanarak projenin tüm kaynaklarını nasıl dengeleyeceğinizi gösterir.

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");

var levelingResult = ResourceLeveler.LevelAll(project);

foreach (var task in levelingResult.AffectedTasks)
{
    Console.WriteLine("Task affected by the leveling operation: " + task.Name);
}

project.Save(OutDir + "Software Development Plan.leveled.mpp");
ResourceLeveler.ClearLeveling(project);

Console.WriteLine("Leveling cleared");
```

### Ayrıca Bakınız

* class [Project](../../../aspose.tasks/project/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)

---

## ClearLeveling(IEnumerable&lt;Task&gt;) {#clearleveling_1}

Kaynak dengelemesi sırasında belirtilen görevlere daha önce eklenmiş olan herhangi bir dengeleme gecikmesini temizler.

```csharp
public static void ClearLeveling(IEnumerable<Task> tasks)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| görevler | IEnumerable`1 | Dengeleme gecikmesinin temizlenmesi gereken görevleri içeren enumerable. |

### Ayrıca Bakınız

* class [Task](../../../aspose.tasks/task/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)


