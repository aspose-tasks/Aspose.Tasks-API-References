---
title: "Rsc.Id"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Kaynaklar listesinde bir kaynağın konum tanımlayıcısı."
type: docs
weight: 350
url: /tr/net/aspose.tasks/rsc/id/
---
## Rsc.Id field

Kaynaklar listesinde bir kaynağın konum tanımlayıcısı.

```csharp
public static readonly Key<int, RscKey> Id;
```

## Örnekler

Rsc.Id özelliğini nasıl okuyup yazacağını gösterir.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Id, 987);

Console.WriteLine("Id: " + resource.Get(Rsc.Id));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


