---
title: "Notlar"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Bir kaynakla ilişkili metin notları."
type: docs
weight: 470
url: /tr/net/aspose.tasks/rsc/notes/
---
## Rsc.Notes field

Bir kaynakla ilişkili metin notları.

```csharp
public static readonly Key<string, RscKey> Notes;
```

### Örnekler

Rsc.Notes özelliğini nasıl okuma/yazma yapılacağını gösterir.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Notes, "Resource Notes");

Console.WriteLine("Notes: " + resource.Get(Rsc.Notes));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2)
* enum [RscKey](../../rsckey)
* class [Rsc](../../rsc)
* namespace [Aspose.Tasks](../../rsc)
* assembly [Aspose.Tasks](../../../)

<!-- DÜZENLEMEYİN: xmldocmd tarafından Aspose.Tasks.dll için oluşturuldu -->
