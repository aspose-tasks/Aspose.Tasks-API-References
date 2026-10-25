---
title: "WorkingTime.Equals"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo WorkingTime. Verifica che gli oggetti siano uguali"
type: docs
weight: 40
url: /it/net/aspose.tasks/workingtime/equals/
---
## WorkingTime.Equals method

Verifica che gli oggetti siano uguali.

```csharp
public override bool Equals(object obj)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | Oggetto | Secondo oggetto da confrontare. |

### Valore di ritorno

True se gli oggetti sono uguali, false altrimenti.

## Esempi

Mostra come verificare l'uguaglianza del tempo di lavoro.

```csharp
var workingTime1 = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 17);

// L'uguaglianza dei calendari è verificata rispetto alle date di inizio e fine del tempo di lavoro.
Console.WriteLine("Working Time 1 (From): " + workingTime1.From);
Console.WriteLine("Working Time 1 (To): " + workingTime1.To);

Console.WriteLine("Working Time 2 (From): " + workingTime2.From);
Console.WriteLine("Working Time 2 (To): " + workingTime2.To);
Console.WriteLine("Are working times equal: " + workingTime1.Equals(workingTime2));
```

### Vedi anche

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)


