---
title: "OutlineCode.FieldId"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti OutlineCode. Mendapatkan atau mengatur nilai numerik dari bidang khusus Id proyek"
type: docs
weight: 20
url: /id/net/aspose.tasks/outlinecode/fieldid/
---
## OutlineCode.FieldId property

Mendapatkan atau mengatur nilai numerik dari bidang khusus Id proyek.

```csharp
public string FieldId { get; set; }
```

## Contoh

Menampilkan cara membaca kode outline tugas.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// baca kode outline
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

### Lihat Juga

* class [OutlineCode](../)
* namespace [Aspose.Tasks](../../outlinecode/)
* assembly [Aspose.Tasks](../../../)


