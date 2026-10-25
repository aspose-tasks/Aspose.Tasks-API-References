---
title: "Asn.NotesRTF"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Asn. Catatan teks dalam format RTF. Hanya didukung untuk format MPP"
type: docs
weight: 340
url: /id/net/aspose.tasks/asn/notesrtf/
---
## Asn.NotesRTF field

Catatan teks dalam format RTF. Hanya didukung untuk format MPP.

```csharp
public static readonly Key<string, AsnKey> NotesRTF;
```

## Contoh

Menampilkan cara mengambil/mengatur catatan penugasan sumber daya.

```csharp
var project = new Project(DataDir + "UpdateResourceAssignment.mpp");
var task = project.RootTask.Children.GetById(1);
var rsc = project.Resources.GetById(1);

// buat penugasan sumber daya
var assn = project.ResourceAssignments.Add(task, rsc);

// atur catatan penugasan sumber daya 
assn.Set(Asn.NotesText, "Newly added assignment");

Console.WriteLine("Notes text: " + assn.Get(Asn.NotesText));
Console.WriteLine("Notes RTF: " + assn.Get(Asn.NotesRTF));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


