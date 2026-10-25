---
title: "Tsk.Hyperlink"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Judul atau teks penjelas untuk hyperlink yang terkait dengan tugas."
type: docs
weight: 490
url: /id/net/aspose.tasks/tsk/hyperlink/
---
## Tsk.Hyperlink field

Judul atau teks penjelasan untuk hyperlink yang terkait dengan sebuah tugas.

```csharp
public static readonly Key<string, TaskKey> Hyperlink;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.Hyperlink.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Hyperlink, "Click here to visit our site");
task.Set(Tsk.HyperlinkAddress, "https://products.aspose.com");
task.Set(Tsk.HyperlinkSubAddress, "/total/net");

Console.WriteLine("Hyperlink: " + task.Get(Tsk.Hyperlink));
Console.WriteLine("Hyperlink Address: " + task.Get(Tsk.HyperlinkAddress));
Console.WriteLine("Hyperlink Sub Address: " + task.Get(Tsk.HyperlinkSubAddress));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


