---
title: "Asn.Resume"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Asn. La date à laquelle l'affectation est reprise"
type: docs
weight: 490
url: /fr/net/aspose.tasks/asn/resume/
---
## Asn.Resume field

La date à laquelle l'affectation est reprise.

```csharp
public static readonly Key<DateTime, AsnKey> Resume;
```

## Exemples

Montre comment lire les dates d'arrêt/reprise de l'affectation.

```csharp
var project = new Project(DataDir + "ResourceAssignmentStopResumeDates.mpp");

// Imprimer les dates d'arrêt et de reprise de l'affectation de ressource
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.Stop).ToShortDateString() == "1/1/2000" ? "NA" : ra.Get(Asn.Stop).ToShortDateString());
    Console.WriteLine(ra.Get(Asn.Resume).ToShortDateString() == "1/1/2000" ? "NA" : ra.Get(Asn.Resume).ToShortDateString());
}
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


