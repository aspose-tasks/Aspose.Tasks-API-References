---
title: "Rsc.AssignmentOwnerGuid"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Bir atama sahibinin GUID'i"
type: docs
weight: 110
url: /tr/net/aspose.tasks/rsc/assignmentownerguid/
---
## Rsc.AssignmentOwnerGuid field

Bir atama sahibinin GUID'i.

```csharp
public static readonly Key<string, RscKey> AssignmentOwnerGuid;
```

## Örnekler

Rsc.AssignmentOwnerGuid özelliğini okuma/yazma nasıl yapılacağını gösterir.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AssignmentOwnerGuid, "aad9ac22-9f06-4196-906b-916acebcc1c2");

Console.WriteLine("Assignment Owner Guid: " + resource.Get(Rsc.AssignmentOwnerGuid));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


