---
title: "Kelas OutlineCode"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.OutlineCode class. Mewakili nilai dari kode outline"
type: docs
weight: 1150
url: /id/net/aspose.tasks/outlinecode/
---
## OutlineCode class

Mewakili nilai dari kode outline.

```csharp
public class OutlineCode
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [OutlineCode](outlinecode/#constructor)() | Menginisialisasi instance baru dari kelas `OutlineCode`. |
| [OutlineCode](outlinecode/#constructor_1)(OutlineCodeDefinition, OutlineValue) | Menginisialisasi instance baru dari kelas `OutlineCode` menggunakan Outline Code yang ditentukan dan salah satu nilainya. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [FieldId](../../aspose.tasks/outlinecode/fieldid/) { get; set; } | Mendapatkan atau mengatur nilai numerik dari bidang khusus Id proyek. |
| [ValueGuid](../../aspose.tasks/outlinecode/valueguid/) { get; set; } | Mendapatkan atau mengatur GUID dari nilai dalam daftar nilai. ValueGuid cocok dengan FieldGuid dalam daftar nilai. |
| [ValueId](../../aspose.tasks/outlinecode/valueid/) { get; set; } | Mendapatkan atau mengatur Id dalam daftar nilai yang terkait dengan definisi dalam koleksi kode outline. |

## Catatan

Dua potongan data diperlukan - sebuah penunjuk ke tabel kode outline yang ditentukan oleh FieldId, dan nilai yang ditentukan baik oleh penunjuk ValueId atau ValueGuid ke daftar nilai.

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


