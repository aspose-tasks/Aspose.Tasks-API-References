---
title: "VbaReference.Equals"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode VbaReference. Retourne une valeur indiquant si cette instance est égale à l'objet VbaReference spécifié"
type: docs
weight: 40
url: /fr/net/aspose.tasks/vbareference/equals/
---
## Equals(VbaReference) {#equals}

Retourne une valeur indiquant si cette instance est égale à l'objet [`VbaReference`](../) spécifié.

```csharp
public bool Equals(VbaReference other)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| other | VbaReference | L'objet [`VbaReference`](../) spécifié à comparer avec cette instance. |

### Valeur de retour

Retourne true si cette instance est égale à l'objet [`VbaReference`](../) spécifié; sinon, false.

## Exemples

Montre comment vérifier l'égalité d'une référence VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

var reference1 = project.VbaProject.References.ToList()[0];
var reference2 = project.VbaProject.References.ToList()[1];

// L'égalité des références est vérifiée par rapport au nom de la référence.
Console.WriteLine("VBA reference 1 Name: " + reference1.Name);
Console.WriteLine("VBA reference 2 Name: " + reference2.Name);
Console.WriteLine("Are references equal: " + reference1.Equals(reference2));
```

### Voir aussi

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Retourne une valeur indiquant si cette instance est égale à l'objet [`VbaReference`](../) spécifié.

```csharp
public override bool Equals(object obj)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| obj | Object | L'objet [`VbaReference`](../) spécifié à comparer avec cette instance. |

### Valeur de retour

Retourne true si cette instance est égale à l'objet [`VbaReference`](../) spécifié; sinon, false.

## Exemples

Montre comment vérifier l'égalité d'une référence VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

var reference1 = project.VbaProject.References.ToList()[0];
var reference2 = project.VbaProject.References.ToList()[1];

// L'égalité des références est vérifiée par rapport au nom de la référence.
Console.WriteLine("VBA reference 1 Name: " + reference1.Name);
Console.WriteLine("VBA reference 2 Name: " + reference2.Name);
Console.WriteLine("Are references equal: " + reference1.Equals(reference2));
```

### Voir aussi

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)


