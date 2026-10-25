---
title: "Prj.Manager"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Bir projenin yöneticisi"
type: docs
weight: 450
url: /tr/net/aspose.tasks/prj/manager/
---
## Prj.Manager field

Bir projenin yöneticisi.

```csharp
public static readonly Key<string, PrjKey> Manager;
```

## Örnekler

Prj.Manager özelliğini okuma/yazma yöntemini gösterir.

```csharp
var project = new Project();

project.Set(Prj.Manager, "Steve");

Console.WriteLine("Manager: " + project.Get(Prj.Manager));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


