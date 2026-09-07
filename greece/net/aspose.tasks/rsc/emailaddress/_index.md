---
title: "Rsc.EMailAddress"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Η διεύθυνση email ενός πόρου"
type: docs
weight: 280
url: /el/net/aspose.tasks/rsc/emailaddress/
---
## Rsc.EMailAddress field

Η διεύθυνση email ενός πόρου.

```csharp
public static readonly Key<string, RscKey> EMailAddress;
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


