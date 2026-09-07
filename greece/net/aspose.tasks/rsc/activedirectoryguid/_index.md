---
title: "Rsc.ActiveDirectoryGuid"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Το Active Directory Guid για έναν πόρο"
type: docs
weight: 20
url: /el/net/aspose.tasks/rsc/activedirectoryguid/
---
## Rsc.ActiveDirectoryGuid field

Το GUID του Active Directory για έναν πόρο.

```csharp
public static readonly Key<string, RscKey> ActiveDirectoryGuid;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.ActiveDirectoryGuid.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActiveDirectoryGuid, "8aede269-c574-4a8b-aa74-32bc877a2aef");

Console.WriteLine("Active Directory Guid: " + resource.Get(Rsc.ActiveDirectoryGuid));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


