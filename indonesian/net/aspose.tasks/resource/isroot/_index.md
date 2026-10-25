---
title: "Resource.IsRoot"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Resource. Mendapatkan flag yang menunjukkan apakah sumber daya adalah sumber daya root. Sumber daya root adalah sumber daya khusus yang dimaksudkan untuk mendukung internal format MS Projects dan tidak dimaksudkan untuk digunakan langsung dari kode pengguna"
type: docs
weight: 470
url: /id/net/aspose.tasks/resource/isroot/
---
## Resource.IsRoot property

Mendapatkan flag yang menunjukkan apakah sumber daya adalah sumber daya akar. Sumber daya akar adalah sumber daya khusus yang dimaksudkan untuk mendukung internal format MS Project dan tidak dimaksudkan untuk digunakan langsung dari kode pengguna.

```csharp
public virtual bool IsRoot { get; }
```

## Contoh

Menampilkan cara menggunakan properti IsRoot untuk melewati sumber daya root.

```csharp
var project = new Project(DataDir + "ResourceCosts.mpp");

foreach (var resource in project.Resources)
{
    if (resource.IsRoot)
    {
        continue;
    }

    Console.WriteLine(resource.Get(Rsc.Name));
}
```

### Lihat Juga

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


