---
title: Project.RescheduleUncompletedWorkToStartAfter
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: Project metodo. Riprogramma il lavoro del progetto non completato per iniziare dopo una data specificata.
type: docs
weight: 1170
url: /it/net/aspose.tasks/project/rescheduleuncompletedworktostartafter/
---
## RescheduleUncompletedWorkToStartAfter(DateTime) {#rescheduleuncompletedworktostartafter}

Riprogramma il lavoro del progetto non completato per iniziare dopo una data specificata.

```csharp
public void RescheduleUncompletedWorkToStartAfter(DateTime after)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| after | DateTime | La data successiva alla quale riprogrammare il lavoro non completato. |

### Osservazioni

Assicurarsi che il flag Project.CanSplitsInProgressTasks sia impostato su true prima di utilizzare questo metodo.

### Guarda anche

* class [Project](../)
* spazio dei nomi [Aspose.Tasks](../../project/)
* assemblea [Aspose.Tasks](../../../)

---

## RescheduleUncompletedWorkToStartAfter(DateTime, List&lt;Task&gt;) {#rescheduleuncompletedworktostartafter_1}

Riprogramma il lavoro non completato per un elenco specificato di attività da avviare dopo una data specificata.

```csharp
public void RescheduleUncompletedWorkToStartAfter(DateTime after, List<Task> taskCollection)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| after | DateTime | La data successiva alla quale riprogrammare il lavoro non completato. |
| taskCollection | List`1 | Elenco&lt;attività&gt; di attività per cui riprogrammare il lavoro non completato. |

### Osservazioni

Assicurarsi che il flag Project.CanSplitsInProgressTasks sia impostato su true prima di utilizzare questo metodo.

### Guarda anche

* class [Task](../../task/)
* class [Project](../)
* spazio dei nomi [Aspose.Tasks](../../project/)
* assemblea [Aspose.Tasks](../../../)


