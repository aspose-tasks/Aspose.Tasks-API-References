---
title: "NullableBool.GetHashCode"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "NullableBool-methode. Retourneert een hashcode-waarde voor het exemplaar van de NullableBool-klasse"
type: docs
weight: 50
url: /nl/net/aspose.tasks/nullablebool/gethashcode/
---
## NullableBool.GetHashCode method

Retourneert een hashcode-waarde voor het exemplaar van de [`NullableBool`](../) klasse.

```csharp
public override int GetHashCode()
```

### Retourwaarde

retourneert een hashcodewaarde voor dit object.

## Voorbeelden

Toont hoe te werken met &lt;see cref="Aspose.Tasks.NullableBool" /&gt;.GetHashCode-methode.

```csharp
var bool1 = new NullableBool(true);
var bool2 = new NullableBool(true, false);

// de hashcode van booleans is gebaseerd op de 'IsDefined' en 'Value' eigenschappen
Console.WriteLine("Bool 1: {0} Hash Code 1: {1}", bool1.ToString(), bool1.GetHashCode());
Console.WriteLine("Bool 2: {0} Hash Code 1: {1}", bool2.ToString(), bool2.GetHashCode());
```

### Zie ook

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)


