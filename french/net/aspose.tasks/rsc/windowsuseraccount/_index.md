---
title: "Rsc.WindowsUserAccount"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. Le compte NT associé à une ressource"
type: docs
weight: 680
url: /fr/net/aspose.tasks/rsc/windowsuseraccount/
---
## Rsc.WindowsUserAccount field

Le compte NT associé à une ressource.

```csharp
public static readonly Key<string, RscKey> WindowsUserAccount;
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


