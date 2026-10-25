---
title: "Prj.Guid"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. Le GUID du projet"
type: docs
weight: 360
url: /fr/net/aspose.tasks/prj/guid/
---
## Prj.Guid field

Le GUID du projet.

```csharp
public static readonly Key<Guid, PrjKey> Guid;
```

## Exemples

Montre comment lire/écrire la propriété Prj.Guid.

```csharp
var project = new Project();

project.Set(Prj.Guid, new Guid("efcc0d63-d8e0-4a34-9f3e-9f973f50238a"));

Console.WriteLine("Guid: " + project.Get(Prj.Guid));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


