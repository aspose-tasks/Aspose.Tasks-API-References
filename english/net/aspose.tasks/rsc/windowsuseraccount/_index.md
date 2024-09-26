---
title: Rsc.WindowsUserAccount
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. The NT account associated with a resource
type: docs
weight: 680
url: /net/aspose.tasks/rsc/windowsuseraccount/
---
## Rsc.WindowsUserAccount field

The NT account associated with a resource.

```csharp
public static readonly Key<string, RscKey> WindowsUserAccount;
```

## Examples

Shows how to set resource's meta properties.

```csharp
var project = new Project(DataDir + "Project.mpp");

// Add resource and set resource meta data
var resource = project.Resources.Add("Rsc 1");
resource.Set(Rsc.EMailAddress, "1@gmail.com");
resource.Set(Rsc.WindowsUserAccount, "user_acc1");
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


