---
title: "VbaModuleAttribute.Equals"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode VbaModuleAttribute. Retourne une valeur indiquant si cette instance est égale à l'objet VbaModuleAttribute spécifié"
type: docs
weight: 30
url: /fr/net/aspose.tasks/vbamoduleattribute/equals/
---
## Equals(VbaModuleAttribute) {#equals}

Retourne une valeur indiquant si cette instance est égale à l'objet [`VbaModuleAttribute`](../) spécifié.

```csharp
public bool Equals(VbaModuleAttribute other)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| other | VbaModuleAttribute | L'objet [`VbaModuleAttribute`](../) spécifié à comparer avec cette instance. |

### Valeur de retour

Retourne true si cette instance est égale à l'objet [`VbaModuleAttribute`](../) spécifié ; sinon, false.

## Exemples

Montre comment vérifier l'égalité des attributs de module VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var module = project.VbaProject.Modules.ToList()[0];

var attribute1 = module.Attributes.ToList()[0];
var attribute2 = module.Attributes.ToList()[0];
Console.WriteLine("Module attribute 1 Key: {0}, Value: {1}", attribute1.Key, attribute1.Value);
Console.WriteLine("Module attribute 2 Key: {0}, Value: {1}", attribute2.Key, attribute2.Value);
Console.WriteLine("Are module attributes equal: " + attribute1.Equals(attribute2));
```

### Voir aussi

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Retourne une valeur indiquant si cette instance est égale à l'objet [`VbaModuleAttribute`](../) spécifié.

```csharp
public override bool Equals(object obj)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| obj | Object | L'objet [`VbaModuleAttribute`](../) spécifié à comparer avec cette instance. |

### Valeur de retour

Retourne true si cette instance est égale à l'objet [`VbaModuleAttribute`](../) spécifié ; sinon, false.

## Exemples

Montre comment vérifier l'égalité des attributs de module VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var module = project.VbaProject.Modules.ToList()[0];

var attribute1 = module.Attributes.ToList()[0];
var attribute2 = module.Attributes.ToList()[0];
Console.WriteLine("Module attribute 1 Key: {0}, Value: {1}", attribute1.Key, attribute1.Value);
Console.WriteLine("Module attribute 2 Key: {0}, Value: {1}", attribute2.Key, attribute2.Value);
Console.WriteLine("Are module attributes equal: " + attribute1.Equals(attribute2));
```

### Voir aussi

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)


