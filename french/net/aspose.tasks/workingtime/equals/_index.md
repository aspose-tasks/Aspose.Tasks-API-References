---
title: "WorkingTime.Equals"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode WorkingTime. Vérifie que les objets sont égaux"
type: docs
weight: 40
url: /fr/net/aspose.tasks/workingtime/equals/
---
## WorkingTime.Equals method

Vérifie que les objets sont égaux.

```csharp
public override bool Equals(object obj)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| obj | Objet | Second objet à comparer. |

### Valeur de retour

Vrai si les objets sont égaux, faux sinon.

## Exemples

Montre comment vérifier l'égalité du temps de travail.

```csharp
var workingTime1 = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 17);

// L'égalité des calendriers est vérifiée par rapport aux dates de début et de fin du temps de travail.
Console.WriteLine("Working Time 1 (From): " + workingTime1.From);
Console.WriteLine("Working Time 1 (To): " + workingTime1.To);

Console.WriteLine("Working Time 2 (From): " + workingTime2.From);
Console.WriteLine("Working Time 2 (To): " + workingTime2.To);
Console.WriteLine("Are working times equal: " + workingTime1.Equals(workingTime2));
```

### Voir aussi

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)


