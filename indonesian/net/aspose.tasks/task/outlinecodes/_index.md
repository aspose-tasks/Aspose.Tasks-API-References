---
title: "Task.OutlineCodes"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Task. Mendapatkan atau mengatur objek OutlineCodeCollection"
type: docs
weight: 880
url: /id/net/aspose.tasks/task/outlinecodes/
---
## Task.OutlineCodes property

Mendapatkan atau mengatur objek [`OutlineCodeCollection`](../../outlinecodecollection/).

```csharp
public OutlineCodeCollection OutlineCodes { get; set; }
```

## Catatan

Dua potongan data diperlukan - sebuah pointer ke tabel kode outline yang ditentukan oleh FieldID, dan nilai yang ditentukan baik oleh pointer ValueID atau ValueGUID ke daftar nilai.

## Contoh

Tunjukkan cara membaca nilai kode outline tugas.

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

### Lihat Juga

* class [OutlineCodeCollection](../../outlinecodecollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


