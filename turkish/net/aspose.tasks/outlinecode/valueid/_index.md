---
title: "OutlineCode.ValueId"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "OutlineCode özelliği. Outline code koleksiyonundaki tanımla ilişkili değer listesinde Id'yi alır veya ayarlar"
type: docs
weight: 40
url: /tr/net/aspose.tasks/outlinecode/valueid/
---
## OutlineCode.ValueId property

Outline kod koleksiyonundaki tanımlama ile ilişkili değer listesindeki Id'yi alır veya ayarlar.

```csharp
public int ValueId { get; set; }
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


