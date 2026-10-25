---
title: "Resource.GetHashCode"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Resource method. Restituisce un valore di codice hash per l'istanza della classe Resource"
type: docs
weight: 840
url: /it/net/aspose.tasks/resource/gethashcode/
---
## Resource.GetHashCode method

Restituisce un valore di codice hash per l'istanza della classe [`Resource`](../).

```csharp
public override int GetHashCode()
```

### Valore di ritorno

restituisce un valore di hash per questo oggetto.

## Esempi

Mostra come ottenere un codice hash di una risorsa.

```csharp
var project = new Project(DataDir + "Project.mpp");

var resource1 = project.Resources.GetById(1);
var resource2 = project.Resources.GetById(2);

// Il codice hash di una risorsa è uguale all'UID della risorsa 
Console.WriteLine("Resource UID: {0} Hash Code: {1}", resource1.Get(Rsc.Uid), resource1.GetHashCode());
Console.WriteLine("Resource UID: {0} Hash Code: {1}", resource2.Get(Rsc.Uid), resource2.GetHashCode());
```

### Vedi anche

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


