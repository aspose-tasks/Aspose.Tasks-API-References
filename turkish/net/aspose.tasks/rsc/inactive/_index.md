---
title: "Rsc.Inactive"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Bir kaynağın yönetim haklarına sahip bir kullanıcı tarafından devre dışı bırakılıp bırakılmadığını belirler"
type: docs
weight: 360
url: /tr/net/aspose.tasks/rsc/inactive/
---
## Rsc.Inactive field

Bir kaynağın yönetici yetkisine sahip bir kullanıcı tarafından devre dışı bırakılıp bırakılmadığını belirler.

```csharp
public static readonly Key<NullableBool, RscKey> Inactive;
```

## Örnekler

Rsc.Inactive özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Inactive, true);

Console.WriteLine("Inactive: " + resource.Get(Rsc.Inactive));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


