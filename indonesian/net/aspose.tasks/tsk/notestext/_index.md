---
title: "Tsk.NotesText"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Catatan teks biasa yang diekstrak dari data RTF."
type: docs
weight: 830
url: /id/net/aspose.tasks/tsk/notestext/
---
## Tsk.NotesText field

Teks polos catatan yang diekstrak dari data RTF.

```csharp
public static readonly Key<string, TaskKey> NotesText;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.NotesText.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.NotesText, "Notes");

Console.WriteLine("Notes Text: " + task.Get(Tsk.NotesText));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


