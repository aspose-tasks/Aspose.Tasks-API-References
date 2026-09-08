---
title: "Rsc.EMailAddress"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc field. Het e‑mailadres van een resource"
type: docs
weight: 280
url: /nl/net/aspose.tasks/rsc/emailaddress/
---
## Rsc.EMailAddress field

Het e-mailadres van een resource.

```csharp
public static readonly Key<string, RscKey> EMailAddress;
```

## Voorbeelden

Toont hoe de meta-eigenschappen van een resource in te stellen.

```csharp
var project = new Project(DataDir + "Project.mpp");

// Resource toevoegen en resource-metadata instellen.
var resource = project.Resources.Add("Rsc 1");
resource.Set(Rsc.EMailAddress, "1@gmail.com");
resource.Set(Rsc.WindowsUserAccount, "user_acc1");
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


