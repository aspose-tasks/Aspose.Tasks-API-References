---
title: "Prj.Company"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alan. Bir projenin oluşturulduğu şirket."
type: docs
weight: 120
url: /tr/net/aspose.tasks/prj/company/
---
## Prj.Company field

Projenin oluşturulduğu şirket.

```csharp
public static readonly Key<string, PrjKey> Company;
```

## Örnekler

Prj.Company özelliğini nasıl okuyup yazacağınızı gösterir.

```csharp
var project = new Project();

project.Set(Prj.Company, "Aspose");

Console.WriteLine("Company: " + project.Get(Prj.Company));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


