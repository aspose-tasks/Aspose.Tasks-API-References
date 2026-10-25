---
title: "Rsc.ActiveDirectoryGuid"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. Le Guid Active Directory d’une ressource"
type: docs
weight: 20
url: /fr/net/aspose.tasks/rsc/activedirectoryguid/
---
## Rsc.ActiveDirectoryGuid field

Le GUID Active Directory d'une ressource.

```csharp
public static readonly Key<string, RscKey> ActiveDirectoryGuid;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.ActiveDirectoryGuid.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActiveDirectoryGuid, "8aede269-c574-4a8b-aa74-32bc877a2aef");

Console.WriteLine("Active Directory Guid: " + resource.Get(Rsc.ActiveDirectoryGuid));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


