---
title: "Project.RemoveInvalidResourceAssignments"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Project. Menghilangkan penugasan sumber daya yang tidak valid dari daftar penugasan sumber daya proyek."
type: docs
weight: 1170
url: /id/net/aspose.tasks/project/removeinvalidresourceassignments/
---
## Project.RemoveInvalidResourceAssignments method

Menghapus penugasan sumber daya yang tidak valid dari daftar penugasan sumber daya proyek.

```csharp
public void RemoveInvalidResourceAssignments()
```

## Catatan

MS Project membuat penugasan sumber daya kosong untuk setiap tugas. Panggil metode tersebut untuk menghapusnya.

## Contoh

Menampilkan cara menghapus penugasan yang tidak valid.

```csharp
var project = new Project(DataDir + "InvalidResourceAssignments.mpp");
var invalid = 0;

// ReSharper disable once LoopCanBeConvertedToQuery //ExSkip
foreach (var ra in project.ResourceAssignments)
{
    if (ra.Get(Asn.Resource) == null)
    {
        invalid++;
    }
}

Console.WriteLine("Count of invalid assignments (before): " + invalid);

// hapus penugasan yang tidak valid
project.RemoveInvalidResourceAssignments();

Console.WriteLine("Count of invalid assignments (after): " + invalid);
```

### Lihat Juga

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


