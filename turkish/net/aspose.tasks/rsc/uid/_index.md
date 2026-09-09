---
title: "Rsc.Uid"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Bir kaynağın benzersiz tanımlayıcısı"
type: docs
weight: 670
url: /tr/net/aspose.tasks/rsc/uid/
---
## Rsc.Uid field

Bir kaynağın benzersiz tanımlayıcısı.

```csharp
public static readonly Key<int, RscKey> Uid;
```

## Örnekler

Rsc.Uid özelliğini nasıl okuma/yazma yapılacağını gösterir.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Uid, 99);

Console.WriteLine("Uid: " + resource.Get(Rsc.Uid));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


