---
title: "Rsc.Workgroup"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Bir kaynağın ait olduğu iş grubunun türü."
type: docs
weight: 700
url: /tr/net/aspose.tasks/rsc/workgroup/
---
## Rsc.Workgroup field

Bir kaynağın ait olduğu iş grubunun türü.

```csharp
public static readonly Key<WorkGroupType, RscKey> Workgroup;
```

## Örnekler

Rsc.Workgroup özelliğini okuma/yazma nasıl yapılacağını gösterir.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Workgroup, WorkGroupType.Email);

Console.WriteLine("Workgroup: " + resource.Get(Rsc.Workgroup));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [WorkGroupType](../../workgrouptype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


