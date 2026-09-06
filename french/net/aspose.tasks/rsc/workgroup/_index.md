---
title: "Rsc.Workgroup"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. Le type de groupe de travail auquel appartient une ressource"
type: docs
weight: 700
url: /fr/net/aspose.tasks/rsc/workgroup/
---
## Rsc.Workgroup field

Le type d'un groupe de travail auquel appartient une ressource.

```csharp
public static readonly Key<WorkGroupType, RscKey> Workgroup;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.Workgroup.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Workgroup, WorkGroupType.Email);

Console.WriteLine("Workgroup: " + resource.Get(Rsc.Workgroup));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [WorkGroupType](../../workgrouptype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


