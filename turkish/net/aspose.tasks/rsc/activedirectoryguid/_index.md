---
title: "Rsc.ActiveDirectoryGuid"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Bir kaynak için Active Directory Guid'i"
type: docs
weight: 20
url: /tr/net/aspose.tasks/rsc/activedirectoryguid/
---
## Rsc.ActiveDirectoryGuid field

Bir kaynak için Active Directory Guid'i.

```csharp
public static readonly Key<string, RscKey> ActiveDirectoryGuid;
```

## Örnekler

Rsc.ActiveDirectoryGuid özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActiveDirectoryGuid, "8aede269-c574-4a8b-aa74-32bc877a2aef");

Console.WriteLine("Active Directory Guid: " + resource.Get(Rsc.ActiveDirectoryGuid));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


