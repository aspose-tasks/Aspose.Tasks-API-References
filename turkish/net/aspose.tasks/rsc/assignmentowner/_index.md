---
title: "Rsc.AssignmentOwner"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Bir atama sahibinin adı."
type: docs
weight: 100
url: /tr/net/aspose.tasks/rsc/assignmentowner/
---
## Rsc.AssignmentOwner field

Bir atama sahibinin adı.

```csharp
public static readonly Key<string, RscKey> AssignmentOwner;
```

## Örnekler

Rsc.AssignmentOwner özelliğini okuma/yazma nasıl yapılacağını gösterir.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AssignmentOwner, "John");

Console.WriteLine("Assignment Owner: " + resource.Get(Rsc.AssignmentOwner));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


