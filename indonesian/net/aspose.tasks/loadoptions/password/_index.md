---
title: "LoadOptions.Password"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti LoadOptions. Mendapatkan atau mengatur kata sandi perlindungan."
type: docs
weight: 50
url: /id/net/aspose.tasks/loadoptions/password/
---
## LoadOptions.Password property

Mendapatkan atau mengatur kata sandi perlindungan.

```csharp
public string Password { get; set; }
```

## Contoh

Menampilkan cara memuat proyek yang dilindungi kata sandi menggunakan instance &lt;see cref="Aspose.Tasks.LoadOptions"/&gt;.

```csharp
using (var stream = new FileStream(DataDir + "PasswordProtectedProject.mpp", FileMode.Open))
{
    var options = new LoadOptions
    {
        Password = "password"
    };
    var project = new Project(stream, options);
    Console.WriteLine(project.Get(Prj.Name));
}
```

### Lihat Juga

* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


