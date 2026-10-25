---
title: "ResourceAssignment.Equals"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo ResourceAssignment. Restituisce un valore che indica se questa istanza è uguale a una specifica istanza della classe ResourceAssignment"
type: docs
weight: 690
url: /it/net/aspose.tasks/resourceassignment/equals/
---
## Equals(ResourceAssignment) {#equals}

Restituisce un valore che indica se questa istanza è uguale a una specifica istanza della classe [`ResourceAssignment`](../).

```csharp
public bool Equals(ResourceAssignment other)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| other | ResourceAssignment | L'istanza specificata della classe [`ResourceAssignment`](../) da confrontare con questa istanza. |

### Valore di ritorno

**True** if the specified instance of the [`ResourceAssignment`](../) class has the same UID value as this instance; otherwise, **false**.

## Esempi

Mostra come verificare l'uguaglianza dell'assegnazione di risorsa.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var resourceAssignment1 = project.ResourceAssignments.GetByUid(1);
var resourceAssignment2 = project.ResourceAssignments.GetByUid(1);

Console.WriteLine("Are resource assignments equal: " + resourceAssignment1.Equals(resourceAssignment2));
```

### Vedi anche

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato.

```csharp
public override bool Equals(object obj)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | Oggetto | L'oggetto da confrontare con questa istanza. |

### Valore di ritorno

**True** if o is a ResourceAssignment that assign the same resource and task as this instance; otherwise, **false**.

## Esempi

Mostra come verificare l'uguaglianza dell'assegnazione di risorsa.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var resourceAssignment1 = project.ResourceAssignments.GetByUid(1);
var resourceAssignment2 = project.ResourceAssignments.GetByUid(1);

Console.WriteLine("Are resource assignments equal: " + resourceAssignment1.Equals(resourceAssignment2));
```

### Vedi anche

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


