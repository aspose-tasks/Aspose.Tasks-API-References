---
title: "Prj.Template"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Prj. Template proyek"
type: docs
weight: 720
url: /id/net/aspose.tasks/prj/template/
---
## Prj.Template field

Templat proyek.

```csharp
public static readonly Key<string, PrjKey> Template;
```

## Contoh

Menampilkan cara membaca/menulis properti Prj.Template.

```csharp
var project = new Project();

project.Set(Prj.Template, "Custom Template");

Console.WriteLine("Template: " + project.Get(Prj.Template));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


