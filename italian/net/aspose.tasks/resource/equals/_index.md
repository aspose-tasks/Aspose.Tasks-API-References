---
title: "Resource.Equals"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Resource. Restituisce un valore che indica se questa istanza è uguale a una specifica istanza della classe Resource"
type: docs
weight: 820
url: /it/net/aspose.tasks/resource/equals/
---
## Equals(Resource) {#equals}

Restituisce un valore che indica se questa istanza è uguale a una specifica istanza della classe [`Resource`](../).

```csharp
public bool Equals(Resource other)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| other | Resource | L'istanza specificata della classe [`Resource`](../) da confrontare con questa istanza. |

### Valore di ritorno

**True** if the specified instance of the [`Resource`](../) class has the same Uid value as this instance; otherwise, **false**.

## Esempi

Mostra come verificare l'uguaglianza della risorsa.

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

var resource1 = project.Resources.GetById(1);
var resource2 = project.Resources.GetById(1);

Console.WriteLine("Are resources equal: " + resource1.Equals(resource2));
```

### Vedi anche

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
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

**True** if the specified object is a Resource that has the same Uid value as this instance; otherwise, **false**.

## Esempi

Mostra come verificare l'uguaglianza della risorsa.

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

var resource1 = project.Resources.GetById(1);
var resource2 = project.Resources.GetById(1);

Console.WriteLine("Are resources equal: " + resource1.Equals(resource2));
```

### Vedi anche

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


