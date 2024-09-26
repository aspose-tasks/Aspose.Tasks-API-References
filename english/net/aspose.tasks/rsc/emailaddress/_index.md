---
title: Rsc.EMailAddress
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. The email address of a resource
type: docs
weight: 280
url: /net/aspose.tasks/rsc/emailaddress/
---
## Rsc.EMailAddress field

The email address of a resource.

```csharp
public static readonly Key<string, RscKey> EMailAddress;
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


