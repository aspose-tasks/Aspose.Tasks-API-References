---
title: "NullableBool.GetHashCode"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode NullableBool. Retourne une valeur de code de hachage pour l'instance de la classe NullableBool"
type: docs
weight: 50
url: /fr/net/aspose.tasks/nullablebool/gethashcode/
---
## NullableBool.GetHashCode method

Retourne une valeur de code de hachage pour l'instance de la classe [`NullableBool`](../).

```csharp
public override int GetHashCode()
```

### Valeur de retour

retourne une valeur de code de hachage pour cet objet.

## Exemples

Montre comment travailler avec la méthode &lt;see cref=\"Aspose.Tasks.NullableBool\" /&gt;.GetHashCode.

```csharp
var bool1 = new NullableBool(true);
var bool2 = new NullableBool(true, false);

// le code de hachage des booléens est basé sur les propriétés 'IsDefined' et 'Value'
Console.WriteLine("Bool 1: {0} Hash Code 1: {1}", bool1.ToString(), bool1.GetHashCode());
Console.WriteLine("Bool 2: {0} Hash Code 1: {1}", bool2.ToString(), bool2.GetHashCode());
```

### Voir aussi

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)


