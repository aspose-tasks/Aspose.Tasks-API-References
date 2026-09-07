---
title: "Tsk.HyperlinkSubAddress"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Lokasi spesifik dalam dokumen pada hyperlink yang terkait dengan tugas."
type: docs
weight: 510
url: /id/net/aspose.tasks/tsk/hyperlinksubaddress/
---
## Tsk.HyperlinkSubAddress field

Lokasi spesifik dalam dokumen pada tautan yang terkait dengan tugas.

```csharp
public static readonly Key<string, TaskKey> HyperlinkSubAddress;
```

## Catatan

Alamat lengkap (Hyperlink Href dalam Microsoft Project) dari hyperlink adalah penggabungan HyperlinkAddress dan HyperlinkSubAddress.

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


