---
title: "Rsc.WindowsUserAccount"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Rsc field. Ο λογαριασμός NT που σχετίζεται με έναν πόρο"
type: docs
weight: 680
url: /el/net/aspose.tasks/rsc/windowsuseraccount/
---
## Rsc.WindowsUserAccount field

Ο λογαριασμός NT που σχετίζεται με έναν πόρο.

```csharp
public static readonly Key<string, RscKey> WindowsUserAccount;
```

## Παραδείγματα

Δείχνει πώς να ορίσετε τις μετα-ιδιότητες του πόρου.

```csharp
var project = new Project(DataDir + "Project.mpp");

// Προσθέστε πόρο και ορίστε μετα-δεδομένα πόρου
var resource = project.Resources.Add("Rsc 1");
resource.Set(Rsc.EMailAddress, "1@gmail.com");
resource.Set(Rsc.WindowsUserAccount, "user_acc1");
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


