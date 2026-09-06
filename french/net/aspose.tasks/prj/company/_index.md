---
title: "Prj.Company"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. L’entreprise où un projet a été créé"
type: docs
weight: 120
url: /fr/net/aspose.tasks/prj/company/
---
## Prj.Company field

L'entreprise où un projet a été créé.

```csharp
public static readonly Key<string, PrjKey> Company;
```

## Exemples

Montre comment lire/écrire la propriété Prj.Company.

```csharp
var project = new Project();

project.Set(Prj.Company, "Aspose");

Console.WriteLine("Company: " + project.Get(Prj.Company));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


