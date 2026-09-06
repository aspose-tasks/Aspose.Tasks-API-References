---
title: "Duration.GetHashCode"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Duration. Renvoie une valeur de code de hachage pour cet objet."
type: docs
weight: 90
url: /fr/net/aspose.tasks/duration/gethashcode/
---
## Duration.GetHashCode method

Renvoie une valeur de code de hachage pour cet objet.

```csharp
public override int GetHashCode()
```

### Valeur de retour

renvoie une valeur de code de hachage pour cette instance de durée.

## Exemples

Montre comment obtenir un code de hachage d'une durée.

```csharp
var project = new Project();

var duration1 = project.GetDuration(1, TimeUnitType.Day);
var duration2 = project.GetDuration(1, TimeUnitType.Day);
var duration3 = project.GetDuration(1, TimeUnitType.Hour);

// le code de hachage d'un calendrier est basé sur le type d'unité de temps et la valeur initiale de la durée.
// ainsi les prochains codes de hachage sont égaux.
Console.WriteLine("Duration 1 Hash Code: {0}", duration1.GetHashCode());
Console.WriteLine("Duration 2 Hash Code: {0}", duration2.GetHashCode());
Console.WriteLine("Are duration's hash codes of duration 1 and duration 2 equal: {0}", duration1.GetHashCode().Equals(duration2.GetHashCode()));

// mais les codes de hachage des durées 1 et 3 ne le sont pas.
Console.WriteLine("Duration 1 Hash Code: {0}", duration1.GetHashCode());
Console.WriteLine("Duration 3 Hash Code: {0}", duration3.GetHashCode());
Console.WriteLine("Are duration's hash codes of duration 1 and duration 2 equal: {0}", duration1.GetHashCode().Equals(duration3.GetHashCode()));
```

### Voir aussi

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


