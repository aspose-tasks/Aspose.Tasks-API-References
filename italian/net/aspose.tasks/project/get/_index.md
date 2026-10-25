---
title: "Project.Get"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo del progetto. Restituisce il valore a cui la proprietà è mappata in questo contenitore"
type: docs
weight: 1080
url: /it/net/aspose.tasks/project/get/
---
## Project.Get&lt;T&gt; method

Restituisce il valore a cui la proprietà è mappata in questo contenitore.

```csharp
public T Get<T>(Key<T, PrjKey> key)
```

| Parametro | Descrizione |
| --- | --- |
| T | il tipo del valore mappato. |
| key | la chiave della proprietà specificata. [`Prj`](../../prj/) per ottenere la chiave della proprietà. |

### Valore di ritorno

il valore a cui la proprietà è mappata in questo contenitore.

## Esempi

Mostra come verificare la versione di un progetto.

```csharp
var project = new Project(DataDir + "DetermineProjectVersion.mpp");

// Visualizza versione del progetto
Console.WriteLine("Project Version : " + project.Get(Prj.SaveVersion));
Console.WriteLine("Last Saved : " + project.Get(Prj.LastSaved).ToShortDateString());
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


