---
title: "Sınıf OutlineCode"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.OutlineCode sınıfı. Bir outline kodunun değerini temsil eder"
type: docs
weight: 1150
url: /tr/net/aspose.tasks/outlinecode/
---
## OutlineCode class

Bir ana hat kodunun değerini temsil eder.

```csharp
public class OutlineCode
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [OutlineCode](outlinecode/#constructor)() | `OutlineCode` sınıfının yeni bir örneğini başlatır. |
| [OutlineCode](outlinecode/#constructor_1)(OutlineCodeDefinition, OutlineValue) | Belirtilen Outline Code ve onun değerlerinden birini kullanarak `OutlineCode` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [FieldId](../../aspose.tasks/outlinecode/fieldid/) { get; set; } | Proje Id özel alanının sayısal değerini alır veya ayarlar. |
| [ValueGuid](../../aspose.tasks/outlinecode/valueguid/) { get; set; } | Değer listesindeki değerin GUID'ini alır veya ayarlar. ValueGuid, değer listesindeki FieldGuid ile eşleşir. |
| [ValueId](../../aspose.tasks/outlinecode/valueid/) { get; set; } | Outline kod koleksiyonundaki tanımlama ile ilişkili değer listesindeki Id'yi alır veya ayarlar. |

## Açıklamalar

İki veri parçası gereklidir - FieldId tarafından belirtilen outline kod tablosuna bir işaretçi ve değer listesine ValueId veya ValueGuid işaretçisiyle belirtilen değer.

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


