---
title: "Rsc.Code"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Bir kaynak hakkında kod veya diğer bilgiler"
type: docs
weight: 210
url: /tr/net/aspose.tasks/rsc/code/
---
## Rsc.Code field

Bir kaynak hakkında kod veya diğer bilgiler.

```csharp
public static readonly Key<string, RscKey> Code;
```

## Örnekler

Rsc.Code özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Code, "555292");

Console.WriteLine("Code: " + resource.Get(Rsc.Code));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


