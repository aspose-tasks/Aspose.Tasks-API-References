---
title: "PrimaveraReadOptions.UndefinedConstraintHandlingBehavior"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "PrimaveraReadOptions özelliği. XER formatından okunan tanımsız kısıtlamalara sahip görevleri işlemek için kullanılan davranışı belirtir."
type: docs
weight: 50
url: /tr/net/aspose.tasks/primaverareadoptions/undefinedconstrainthandlingbehavior/
---
## PrimaveraReadOptions.UndefinedConstraintHandlingBehavior property

XER formatından okunan tanımsız kısıtlamalara sahip görevlerin işlenmesinde kullanılan davranışı belirler.

```csharp
public UndefinedConstraintHandlingBehavior UndefinedConstraintHandlingBehavior { get; set; }
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

* enum [UndefinedConstraintHandlingBehavior](../../undefinedconstrainthandlingbehavior/)
* class [PrimaveraReadOptions](../)
* namespace [Aspose.Tasks](../../primaverareadoptions/)
* assembly [Aspose.Tasks](../../../)


