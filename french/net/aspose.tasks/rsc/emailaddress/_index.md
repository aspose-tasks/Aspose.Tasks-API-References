---
title: "Rsc.EMailAddress"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. L'adresse e-mail d'une ressource"
type: docs
weight: 280
url: /fr/net/aspose.tasks/rsc/emailaddress/
---
## Rsc.EMailAddress field

L'adresse e‑mail d'une ressource.

```csharp
public static readonly Key<string, RscKey> EMailAddress;
```

## Exemples

Montre comment définir les méta-propriétés d'une ressource.

```csharp
var project = new Project(DataDir + "Project.mpp");

// Ajouter une ressource et définir les métadonnées de la ressource
var resource = project.Resources.Add("Rsc 1");
resource.Set(Rsc.EMailAddress, "1@gmail.com");
resource.Set(Rsc.WindowsUserAccount, "user_acc1");
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


