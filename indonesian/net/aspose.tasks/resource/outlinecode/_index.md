---
title: "Resource.OutlineCode"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Resource. Mendapatkan objek OutlineCodeCollection. Nilai dari kode outline"
type: docs
weight: 540
url: /id/net/aspose.tasks/resource/outlinecode/
---
## Resource.OutlineCode property

Mendapatkan objek OutlineCodeCollection. Nilai dari kode outline.

```csharp
public OutlineCodeCollection OutlineCode { get; }
```

## Catatan

Dua potongan data diperlukan - sebuah pointer ke tabel kode outline yang ditentukan oleh FieldID, dan nilai yang ditentukan baik oleh pointer ValueID atau ValueGUID ke daftar nilai.

## Contoh

Menampilkan cara bekerja dengan nilai outline sumber daya.

```csharp
var project = new Project(DataDir + "OutlineCodes2003.mpp");

var res = project.Resources.GetById(2);
Assert.AreEqual(2, res.OutlineCode.Count);
foreach (var code in res.OutlineCode)
{
    object val = null;
    foreach (var def in project.OutlineCodes)
    {
        if (def.FieldId != code.FieldId)
        {
            continue;
        }

        foreach (var value in def.Values)
        {
            if (value.ValueId != code.ValueId)
            {
                continue;
            }

            val = value.Value;
            break;
        }
    }

    Console.WriteLine(val.ToString());
}
```

### Lihat Juga

* class [OutlineCodeCollection](../../outlinecodecollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


