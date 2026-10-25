---
title: "Task.OutlineCodes"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Task özelliği. OutlineCodeCollection nesnesini alır veya ayarlar"
type: docs
weight: 880
url: /tr/net/aspose.tasks/task/outlinecodes/
---
## Task.OutlineCodes property

[`OutlineCodeCollection`](../../outlinecodecollection/) nesnesini alır veya ayarlar.

```csharp
public OutlineCodeCollection OutlineCodes { get; set; }
```

## Açıklamalar

İki veri parçası gereklidir - FieldID tarafından belirtilen outline kod tablosuna bir işaretçi ve değerin ValueID veya ValueGUID işaretçisiyle belirtilen değer listesi.

## Örnekler

Görevin taslak kod değerlerini okuma yöntemini göster.

```csharp
var project = new Project(DataDir + "OutlineCodes2003.mpp");
    var mapping = new Dictionary<string, OutlineValueCollection>();

    // ReSharper disable once LoopCanBeConvertedToQuery //ExSkip
    foreach (var code in project.OutlineCodes)
    {
        mapping.Add(code.FieldId, code.Values);
    }

    var task = project.RootTask.Children.GetById(2);
    foreach (var code in task.OutlineCodes)
    {
        var val = GetOutlineValue(mapping[code.FieldId], code.ValueId);
        Console.WriteLine("Outline value: " + val);
    }
}

public static object GetOutlineValue(OutlineValueCollection collection, int valueId)
{
    object obj = null;

    // ReSharper disable once LoopCanBeConvertedToQuery //ExSkip
    foreach (var value in collection)
    {
        if (value.ValueId != valueId)
        {
            continue;
        }

        obj = value.Value;
        break;
    }

    return obj;
}
```

### Ayrıca Bakınız

* class [OutlineCodeCollection](../../outlinecodecollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


