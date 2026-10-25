---
title: "Resource.Equals"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Resource. Retourne une valeur indiquant si cette instance est égale à une instance spécifiée de la classe Resource."
type: docs
weight: 820
url: /fr/net/aspose.tasks/resource/equals/
---
## Equals(Resource) {#equals}

Retourne une valeur indiquant si cette instance est égale à une instance spécifiée de la classe [`Resource`](../).

```csharp
public bool Equals(Resource other)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| other | Resource | L’instance spécifiée de la classe [`Resource`](../) à comparer avec cette instance. |

### Valeur de retour

**True** if the specified instance of the [`Resource`](../) class has the same Uid value as this instance; otherwise, **false**.

## Exemples

Montre comment vérifier l’égalité des ressources.

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

var resource1 = project.Resources.GetById(1);
var resource2 = project.Resources.GetById(1);

Console.WriteLine("Are resources equal: " + resource1.Equals(resource2));
```

### Voir aussi

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Renvoie une valeur indiquant si cette instance est égale à un objet spécifié.

```csharp
public override bool Equals(object obj)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| obj | Objet | L'objet à comparer avec cette instance. |

### Valeur de retour

**True** if the specified object is a Resource that has the same Uid value as this instance; otherwise, **false**.

## Exemples

Montre comment vérifier l’égalité des ressources.

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

var resource1 = project.Resources.GetById(1);
var resource2 = project.Resources.GetById(1);

Console.WriteLine("Are resources equal: " + resource1.Equals(resource2));
```

### Voir aussi

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


