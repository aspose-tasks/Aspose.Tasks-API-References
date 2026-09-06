---
title: "NullableBool.Value"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété NullableBool. Obtient ou définit une valeur indiquant si la valeur actuelle est vraie ou fausse"
type: docs
weight: 30
url: /fr/net/aspose.tasks/nullablebool/value/
---
## NullableBool.Value property

Obtient ou définit une valeur indiquant si la valeur actuelle est vraie ou fausse.

```csharp
public bool Value { get; set; }
```

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

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)


