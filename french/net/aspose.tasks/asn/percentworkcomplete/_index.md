---
title: "Asn.PercentWorkComplete"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Asn. Le montant du travail accompli sur une affectation"
type: docs
weight: 400
url: /fr/net/aspose.tasks/asn/percentworkcomplete/
---
## Asn.PercentWorkComplete field

La quantité de travail terminée sur une affectation.

```csharp
public static readonly Key<int, AsnKey> PercentWorkComplete;
```

## Exemples

Montre comment lire le pourcentage de travail accompli d'une affectation.

```csharp
var project = new Project(DataDir + "ResourceAssignmentPercentWorkComplete.mpp");

// Imprimer le pourcentage d'achèvement de l'affectation
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.PercentWorkComplete).ToString());
}
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


