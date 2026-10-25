---
title: "NullableBool.NullableBool"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Constructeur NullableBool. Initialise une nouvelle instance de la structure NullableBool avec la valeur booléenne spécifiée"
type: docs
weight: 10
url: /fr/net/aspose.tasks/nullablebool/nullablebool/
---
## NullableBool(bool) {#constructor}

Initialise une nouvelle instance de la structure [`NullableBool`](../) avec la valeur booléenne spécifiée.

```csharp
public NullableBool(bool value)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| value | Boolean | la valeur booléenne spécifiée. |

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

---

## NullableBool(bool, bool) {#constructor_1}

Initialise une nouvelle instance de la structure [`NullableBool`](../).

```csharp
public NullableBool(bool value, bool isDefined)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| value | Boolean | La valeur actuelle. |
| isDefined | Boolean | La valeur indiquant si la valeur actuelle est définie. |

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


