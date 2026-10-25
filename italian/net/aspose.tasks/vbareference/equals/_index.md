---
title: "VbaReference.Equals"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo VbaReference. Restituisce un valore che indica se questa istanza è uguale all'oggetto VbaReference specificato"
type: docs
weight: 40
url: /it/net/aspose.tasks/vbareference/equals/
---
## Equals(VbaReference) {#equals}

Restituisce un valore che indica se questa istanza è uguale all'oggetto [`VbaReference`](../) specificato.

```csharp
public bool Equals(VbaReference other)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| other | VbaReference | L'oggetto [`VbaReference`](../) specificato da confrontare con questa istanza. |

### Valore di ritorno

Restituisce true se questa istanza è uguale all'oggetto [`VbaReference`](../) specificato; altrimenti, false.

## Esempi

Mostra come verificare l'uguaglianza del riferimento VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

var reference1 = project.VbaProject.References.ToList()[0];
var reference2 = project.VbaProject.References.ToList()[1];

// L'uguaglianza dei riferimenti viene verificata rispetto al nome del riferimento.
Console.WriteLine("VBA reference 1 Name: " + reference1.Name);
Console.WriteLine("VBA reference 2 Name: " + reference2.Name);
Console.WriteLine("Are references equal: " + reference1.Equals(reference2));
```

### Vedi anche

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Restituisce un valore che indica se questa istanza è uguale all'oggetto [`VbaReference`](../) specificato.

```csharp
public override bool Equals(object obj)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | Object | L'oggetto [`VbaReference`](../) specificato da confrontare con questa istanza. |

### Valore di ritorno

Restituisce true se questa istanza è uguale all'oggetto [`VbaReference`](../) specificato; altrimenti, false.

## Esempi

Mostra come verificare l'uguaglianza del riferimento VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

var reference1 = project.VbaProject.References.ToList()[0];
var reference2 = project.VbaProject.References.ToList()[1];

// L'uguaglianza dei riferimenti viene verificata rispetto al nome del riferimento.
Console.WriteLine("VBA reference 1 Name: " + reference1.Name);
Console.WriteLine("VBA reference 2 Name: " + reference2.Name);
Console.WriteLine("Are references equal: " + reference1.Equals(reference2));
```

### Vedi anche

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)


