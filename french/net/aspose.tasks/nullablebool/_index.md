---
title: "Structure NullableBool"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Structure Aspose.Tasks.NullableBool. Une classe pour les valeurs booléennes avec la possibilité de vérifier si la valeur a été définie ou non."
type: docs
weight: 1110
url: /fr/net/aspose.tasks/nullablebool/
---
## NullableBool structure

Une classe pour les valeurs booléennes avec la possibilité de vérifier si la valeur a été définie ou non.

```csharp
public struct NullableBool : IEquatable<NullableBool>
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [NullableBool](nullablebool/#constructor)(bool) | Initialise une nouvelle instance de la structure `NullableBool` avec la valeur booléenne spécifiée. |
| [NullableBool](nullablebool/#constructor_1)(bool, bool) | Initialise une nouvelle instance de la structure `NullableBool`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [IsDefined](../../aspose.tasks/nullablebool/isdefined/) { get; } | Obtient une valeur indiquant si la valeur a été définie ; sinon, false. |
| [Value](../../aspose.tasks/nullablebool/value/) { get; set; } | Obtient ou définit une valeur indiquant si la valeur actuelle est vraie ou fausse. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Equals](../../aspose.tasks/nullablebool/equals/#equals)(NullableBool) | Renvoie un indicateur indiquant si cette instance est égale à l’instance spécifiée de la classe `NullableBool`. |
| override [Equals](../../aspose.tasks/nullablebool/equals/#equals_1)(object) | Renvoie un indicateur indiquant si cette instance est égale à l'objet spécifié. |
| override [GetHashCode](../../aspose.tasks/nullablebool/gethashcode/)() | Renvoie une valeur de code de hachage pour l’instance de la classe `NullableBool`. |
| override [ToString](../../aspose.tasks/nullablebool/tostring/)() | Renvoie une chaîne qui représente l'objet actuel. |
| [operator ==](../../aspose.tasks/nullablebool/op_equality/) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| [implicit operator](../../aspose.tasks/nullablebool/op_implicit/#op_implicit_1) | Convertit implicitement une instance `NullableBool` en une valeur booléenne. Retourne vrai lorsque [`Value`](./value/) est vrai et que [`IsDefined`](./isdefined/) est vrai. (2 opérateurs) |
| [operator !=](../../aspose.tasks/nullablebool/op_inequality/) | Renvoie une valeur indiquant si cette instance n'est pas égale à un objet spécifié. |

## Exemples

Montre comment travailler avec la classe &lt;see cref=\"NullableBool\" /&gt;.

```csharp
var project = new Project();

// vérifions où la classe <see cref=\"Aspose.Tasks.NullableBool\" /> est utilisée
// l'avantage principal de <see cref=\"Aspose.Tasks.NullableBool\" /> est que 
// on peut le définir comme indéfini lors de la construction
var actualsInSync = new NullableBool(false, false);
Console.WriteLine("'ActualsInSync' Value: " + actualsInSync.Value);
Console.WriteLine("'ActualsInSync' Is Defined: " + actualsInSync.IsDefined);

// ...
// utiliser une instance nullable bool
project.Set(Prj.ActualsInSync, actualsInSync);

// ...
var honorConstraints = new NullableBool(true);
Console.WriteLine("'HonorConstraints' ToString: " + honorConstraints.ToString());

// ...
// utiliser une instance nullable bool
project.Set(Prj.HonorConstraints, honorConstraints);

// ...
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


