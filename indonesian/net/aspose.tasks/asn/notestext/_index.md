---
title: "Asn.NotesText"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Asn. Teks catatan polos yang diekstrak dari data RTF."
type: docs
weight: 350
url: /id/net/aspose.tasks/asn/notestext/
---
## Asn.NotesText field

Teks polos catatan yang diekstrak dari data RTF.

```csharp
public static readonly Key<string, AsnKey> NotesText;
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


