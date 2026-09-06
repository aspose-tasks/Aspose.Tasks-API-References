---
title: "Rsc.AccrueAt"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. Détermine comment et quand les coûts standards et les coûts d'heures supplémentaires de la ressource sont facturés ou imputés au coût d'une tâche"
type: docs
weight: 10
url: /fr/net/aspose.tasks/rsc/accrueat/
---
## Rsc.AccrueAt field

Détermine comment et quand les coûts standards et les coûts supplémentaires des ressources sont facturés, ou imputés, au coût d'une tâche.

```csharp
public static readonly Key<CostAccrualType, RscKey> AccrueAt;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.AccrueAt.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AccrueAt, CostAccrualType.End);

Console.WriteLine("Accrue At: " + resource.Get(Rsc.AccrueAt));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [CostAccrualType](../../costaccrualtype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


