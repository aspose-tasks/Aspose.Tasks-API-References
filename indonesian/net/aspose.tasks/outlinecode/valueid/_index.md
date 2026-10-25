---
title: "OutlineCode.ValueId"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti OutlineCode. Mendapatkan atau mengatur Id dalam daftar nilai yang terkait dengan definisi dalam koleksi kode outline"
type: docs
weight: 40
url: /id/net/aspose.tasks/outlinecode/valueid/
---
## OutlineCode.ValueId property

Mendapatkan atau mengatur Id dalam daftar nilai yang terkait dengan definisi dalam koleksi kode outline.

```csharp
public int ValueId { get; set; }
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


