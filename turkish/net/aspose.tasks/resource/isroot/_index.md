---
title: "Resource.IsRoot"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Resource özelliği. Kaynağın kök kaynak olup olmadığını gösteren bayrağı alır. Kök kaynak, MS Projects biçimlerinin iç işleyişini desteklemek amacıyla tasarlanmış özel bir kaynaktır ve kullanıcı kodundan doğrudan kullanılmak üzere tasarlanmamıştır."
type: docs
weight: 470
url: /tr/net/aspose.tasks/resource/isroot/
---
## Resource.IsRoot property

Kaynağın kök kaynak olup olmadığını gösteren bayrağı alır. Kök kaynak, MS Project formatlarının iç işleyişini desteklemek için tasarlanmış özel bir kaynaktır ve kullanıcının kodundan doğrudan kullanılmak üzere tasarlanmamıştır.

```csharp
public virtual bool IsRoot { get; }
```

## Örnekler

Kök kaynağı atlamak için IsRoot özelliğinin nasıl kullanılacağını gösterir.

```csharp
var project = new Project(DataDir + "ResourceCosts.mpp");

foreach (var resource in project.Resources)
{
    if (resource.IsRoot)
    {
        continue;
    }

    Console.WriteLine(resource.Get(Rsc.Name));
}
```

### Ayrıca Bakınız

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


