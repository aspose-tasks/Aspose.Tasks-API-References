---
title: "ResourceAssignment.Equals"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode ResourceAssignment. Retourne une valeur indiquant si cette instance est égale à une instance spécifiée de la classe ResourceAssignment"
type: docs
weight: 690
url: /fr/net/aspose.tasks/resourceassignment/equals/
---
## Equals(ResourceAssignment) {#equals}

Retourne une valeur indiquant si cette instance est égale à une instance spécifiée de la classe [`ResourceAssignment`](../).

```csharp
public bool Equals(ResourceAssignment other)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| other | ResourceAssignment | L'instance spécifiée de la classe [`ResourceAssignment`](../) à comparer avec cette instance. |

### Valeur de retour

**True** if the specified instance of the [`ResourceAssignment`](../) class has the same UID value as this instance; otherwise, **false**.

## Exemples

Montre comment vérifier l'égalité des affectations de ressources.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var resourceAssignment1 = project.ResourceAssignments.GetByUid(1);
var resourceAssignment2 = project.ResourceAssignments.GetByUid(1);

Console.WriteLine("Are resource assignments equal: " + resourceAssignment1.Equals(resourceAssignment2));
```

### Voir aussi

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
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

**True** if o is a ResourceAssignment that assign the same resource and task as this instance; otherwise, **false**.

## Exemples

Montre comment vérifier l'égalité des affectations de ressources.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var resourceAssignment1 = project.ResourceAssignments.GetByUid(1);
var resourceAssignment2 = project.ResourceAssignments.GetByUid(1);

Console.WriteLine("Are resource assignments equal: " + resourceAssignment1.Equals(resourceAssignment2));
```

### Voir aussi

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


