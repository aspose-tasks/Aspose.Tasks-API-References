---
title: "PrimaveraReadOptions.PreserveUids"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "PrimaveraReadOptions özelliği. Varlıkların özgün benzersiz tanımlayıcılarının korunup korunmayacağını belirten bir bayrağı alır veya ayarlar."
type: docs
weight: 20
url: /tr/net/aspose.tasks/primaverareadoptions/preserveuids/
---
## PrimaveraReadOptions.PreserveUids property

Varlıkların orijinal benzersiz tanımlayıcılarının korunup korunmayacağını belirten bir bayrağı alır veya ayarlar.

```csharp
public bool PreserveUids { get; set; }
```

## Örnekler

Belirtilen Id ile Primavera projesini &lt;see cref="LoadOptions" /&gt; kullanarak nasıl yükleyeceğini gösterir.

```csharp
var loadOptions = new LoadOptions();

var primaveraOptions = new PrimaveraReadOptions()
{
    ProjectUid = 3882,
    UndefinedConstraintHandlingBehavior = UndefinedConstraintHandlingBehavior.None,
    PreserveUids = true
};

// Primavera okuma seçeneklerini ayarla
loadOptions.PrimaveraReadOptions = primaveraOptions;

var project = new Project(DataDir + "PrimaveraProject.xml", loadOptions);
Console.WriteLine("Project Name: " + project.Get(Prj.Name));

// projeyle çalış...
```

### Ayrıca Bakınız

* class [PrimaveraReadOptions](../)
* namespace [Aspose.Tasks](../../primaverareadoptions/)
* assembly [Aspose.Tasks](../../../)


