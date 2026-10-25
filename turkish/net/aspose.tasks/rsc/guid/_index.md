---
title: "Rsc.Guid"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Kaynak için oluşturulan benzersiz kimlik kodunu içerir"
type: docs
weight: 310
url: /tr/net/aspose.tasks/rsc/guid/
---
## Rsc.Guid field

Kaynak için oluşturulan benzersiz kimlik kodunu içerir.

```csharp
public static readonly Key<string, RscKey> Guid;
```

## Örnekler

Rsc.Guid özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Guid, "1385689c-2dd1-4114-935b-054beb6fbbbe");

Console.WriteLine("Guid: " + resource.Get(Rsc.Guid));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


