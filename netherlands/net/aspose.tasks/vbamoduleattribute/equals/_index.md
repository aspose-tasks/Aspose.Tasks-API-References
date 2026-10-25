---
title: "VbaModuleAttribute.Equals"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "VbaModuleAttribute methode. Retourneert een waarde die aangeeft of deze instantie gelijk is aan het opgegeven VbaModuleAttribute-object"
type: docs
weight: 30
url: /nl/net/aspose.tasks/vbamoduleattribute/equals/
---
## Equals(VbaModuleAttribute) {#equals}

Retourneert een waarde die aangeeft of deze instantie gelijk is aan het opgegeven [`VbaModuleAttribute`](../) object.

```csharp
public bool Equals(VbaModuleAttribute other)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| other | VbaModuleAttribute | Het opgegeven [`VbaModuleAttribute`](../) object om te vergelijken met deze instantie. |

### Retourwaarde

Retourneert true als deze instantie gelijk is aan het opgegeven [`VbaModuleAttribute`](../) object; anders false.

## Voorbeelden

Toont hoe de gelijkheid van VBA-module-attributen te controleren.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var module = project.VbaProject.Modules.ToList()[0];

var attribute1 = module.Attributes.ToList()[0];
var attribute2 = module.Attributes.ToList()[0];
Console.WriteLine("Module attribute 1 Key: {0}, Value: {1}", attribute1.Key, attribute1.Value);
Console.WriteLine("Module attribute 2 Key: {0}, Value: {1}", attribute2.Key, attribute2.Value);
Console.WriteLine("Are module attributes equal: " + attribute1.Equals(attribute2));
```

### Zie ook

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Retourneert een waarde die aangeeft of deze instantie gelijk is aan het opgegeven [`VbaModuleAttribute`](../) object.

```csharp
public override bool Equals(object obj)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| obj | Object | Het opgegeven [`VbaModuleAttribute`](../) object om te vergelijken met deze instantie. |

### Retourwaarde

Retourneert true als deze instantie gelijk is aan het opgegeven [`VbaModuleAttribute`](../) object; anders false.

## Voorbeelden

Toont hoe de gelijkheid van VBA-module-attributen te controleren.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var module = project.VbaProject.Modules.ToList()[0];

var attribute1 = module.Attributes.ToList()[0];
var attribute2 = module.Attributes.ToList()[0];
Console.WriteLine("Module attribute 1 Key: {0}, Value: {1}", attribute1.Key, attribute1.Value);
Console.WriteLine("Module attribute 2 Key: {0}, Value: {1}", attribute2.Key, attribute2.Value);
Console.WriteLine("Are module attributes equal: " + attribute1.Equals(attribute2));
```

### Zie ook

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)


