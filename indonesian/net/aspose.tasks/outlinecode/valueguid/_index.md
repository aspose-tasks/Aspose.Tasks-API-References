---
title: "OutlineCode.ValueGuid"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti OutlineCode. Mendapatkan atau mengatur GUID dari nilai dalam daftar nilai. ValueGuid cocok dengan FieldGuid dalam daftar nilai"
type: docs
weight: 30
url: /id/net/aspose.tasks/outlinecode/valueguid/
---
## OutlineCode.ValueGuid property

Mendapatkan atau mengatur GUID dari nilai dalam daftar nilai. ValueGuid cocok dengan FieldGuid dalam daftar nilai.

```csharp
public string ValueGuid { get; set; }
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


