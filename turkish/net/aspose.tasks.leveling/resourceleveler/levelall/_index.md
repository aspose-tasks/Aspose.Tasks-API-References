---
title: "ResourceLeveler.LevelAll"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ResourceLeveler yöntemi. Varsayılan dengeleme seçeneklerini kullanarak tüm proje kaynakları için görevleri dengeler."
type: docs
weight: 20
url: /tr/net/aspose.tasks.leveling/resourceleveler/levelall/
---
## ResourceLeveler.LevelAll method

Varsayılan dengeleme seçeneklerini kullanarak projenin tüm kaynakları için görevleri dengeler.

```csharp
public static LevelingResult LevelAll(Project project)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| project | Project | Kaynak dengelemesinin uygulanacağı proje. |

### Dönüş Değeri

Kaynak dengelemesinin sonuçlarını içeren nesne.

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

* class [LevelingResult](../../levelingresult/)
* class [Project](../../../aspose.tasks/project/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)


