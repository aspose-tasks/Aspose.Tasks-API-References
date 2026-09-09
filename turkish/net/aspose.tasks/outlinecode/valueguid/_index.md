---
title: "OutlineCode.ValueGuid"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "OutlineCode özelliği. Değer listesindeki değerin GUID'ini alır veya ayarlar. ValueGuid, değer listesindeki FieldGuid ile eşleşir"
type: docs
weight: 30
url: /tr/net/aspose.tasks/outlinecode/valueguid/
---
## OutlineCode.ValueGuid property

Değer listesindeki değerin GUID'ini alır veya ayarlar. ValueGuid, değer listesindeki FieldGuid ile eşleşir.

```csharp
public string ValueGuid { get; set; }
```

## Örnekler

Görevlerin outline kodlarını nasıl okuyacağınızı gösterir.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// outline kodlarını oku
foreach (var task in project.RootTask.SelectAllChildTasks())
{
    if (task.OutlineCodes.Count <= 0)
    {
        continue;
    }

    Console.WriteLine("Print outline codes of the task: " + task.Get(Tsk.Name));
    foreach (var value in task.OutlineCodes)
    {
        Console.WriteLine("  Field Id: " + value.FieldId);
        Console.WriteLine("  Value Guid: " + value.ValueGuid);
        Console.WriteLine("  Value Id: " + value.ValueId);
    }
}
```

### Ayrıca Bakınız

* class [OutlineCode](../)
* namespace [Aspose.Tasks](../../outlinecode/)
* assembly [Aspose.Tasks](../../../)


