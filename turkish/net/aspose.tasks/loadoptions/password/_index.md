---
title: "LoadOptions.Password"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "LoadOptions özelliği. Bir koruma parolası alır veya ayarlar."
type: docs
weight: 50
url: /tr/net/aspose.tasks/loadoptions/password/
---
## LoadOptions.Password property

Koruma şifresini alır veya ayarlar.

```csharp
public string Password { get; set; }
```

## Örnekler

Şifre korumalı projeyi <see cref=\"Aspose.Tasks.LoadOptions\"/> örneği kullanarak nasıl yükleyeceğinizi gösterir.

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

### Ayrıca Bakınız

* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


