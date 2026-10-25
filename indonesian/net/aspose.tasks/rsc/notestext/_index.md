---
title: "Rsc.NotesText"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Rsc. Teks catatan polos yang diekstrak dari data RTF"
type: docs
weight: 480
url: /id/net/aspose.tasks/rsc/notestext/
---
## Rsc.NotesText field

Teks polos catatan yang diekstrak dari data RTF.

```csharp
public static readonly Key<string, RscKey> NotesText;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.NotesText.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.NotesText, "Resource Notes");

Console.WriteLine("Notes text: " + resource.Get(Rsc.NotesText));
Console.WriteLine("Notes RTF: " + resource.Get(Rsc.NotesRTF));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


