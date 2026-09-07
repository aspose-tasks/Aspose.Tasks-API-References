---
title: "Prj.Company"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Prj. Perusahaan tempat sebuah proyek dibuat"
type: docs
weight: 120
url: /id/net/aspose.tasks/prj/company/
---
## Prj.Company field

Perusahaan tempat proyek dibuat.

```csharp
public static readonly Key<string, PrjKey> Company;
```

## Contoh

Menampilkan cara membaca/menulis properti Prj.Company.

```csharp
var project = new Project();

project.Set(Prj.Company, "Aspose");

Console.WriteLine("Company: " + project.Get(Prj.Company));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


