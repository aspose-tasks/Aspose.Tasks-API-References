---
title: "Rsc.Phonetics"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Kaynak adının fonetik yazımı. Yalnızca Japonca için kullanılabilir."
type: docs
weight: 560
url: /tr/net/aspose.tasks/rsc/phonetics/
---
## Rsc.Phonetics field

Kaynak adının fonetik yazımı. Yalnızca Japonca için kullanılabilir.

```csharp
public static readonly Key<string, RscKey> Phonetics;
```

## Örnekler

Rsc.Phonetics özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Phonetics, "Phonetics");

Console.WriteLine("Phonetics: " + resource.Get(Rsc.Phonetics));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


