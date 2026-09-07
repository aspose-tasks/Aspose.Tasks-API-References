---
title: "Asn.Hyperlink"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Asn. Judul atau teks penjelasan dari hyperlink yang terkait dengan penugasan"
type: docs
weight: 280
url: /id/net/aspose.tasks/asn/hyperlink/
---
## Asn.Hyperlink field

Judul atau teks penjelasan dari tautan hiper yang terkait dengan penugasan.

```csharp
public static readonly Key<string, AsnKey> Hyperlink;
```

## Contoh

Menampilkan cara membaca/menulis properti hyperlink.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Hyperlink, "Click to visit our site");
assignment.Set(Asn.HyperlinkAddress, "https://products.aspose.com");
assignment.Set(Asn.HyperlinkSubAddress, "/total/net");

Console.WriteLine("Hyperlink: " + assignment.Get(Asn.Hyperlink));
Console.WriteLine("Hyperlink Address: " + assignment.Get(Asn.HyperlinkAddress));
Console.WriteLine("Hyperlink Sub Address: " + assignment.Get(Asn.HyperlinkSubAddress));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


