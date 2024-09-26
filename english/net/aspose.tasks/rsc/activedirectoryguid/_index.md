---
title: Rsc.ActiveDirectoryGuid
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. The Active Directory Guid for a resource
type: docs
weight: 20
url: /net/aspose.tasks/rsc/activedirectoryguid/
---
## Rsc.ActiveDirectoryGuid field

The Active Directory Guid for a resource.

```csharp
public static readonly Key<string, RscKey> ActiveDirectoryGuid;
```

## Examples

Shows how to read/write Rsc.ActiveDirectoryGuid property.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActiveDirectoryGuid, "8aede269-c574-4a8b-aa74-32bc877a2aef");

Console.WriteLine("Active Directory Guid: " + resource.Get(Rsc.ActiveDirectoryGuid));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


