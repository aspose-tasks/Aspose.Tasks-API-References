---
title: "LoadOptions.PrimaveraReadOptions"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "LoadOptions özelliği. Primavera P6 XER veya Primavera P6 Xml formatlarını yükleme davranışını özelleştirmek için kullanılabilen PrimaveraReadOptions sınıfının belirtilen bir örneğini alır veya ayarlar"
type: docs
weight: 60
url: /tr/net/aspose.tasks/loadoptions/primaverareadoptions/
---
## LoadOptions.PrimaveraReadOptions property

Belirtilen bir [`PrimaveraReadOptions`](../../primaverareadoptions/) sınıfının örneğini alır veya ayarlar; bu, Primavera formatlarını (Primavera P6 XER veya Primavera P6 Xml) yükleme davranışını özelleştirmek için kullanılabilir.

```csharp
public PrimaveraReadOptions PrimaveraReadOptions { get; set; }
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

* class [PrimaveraReadOptions](../../primaverareadoptions/)
* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


