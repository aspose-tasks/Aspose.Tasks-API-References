---
title: Add
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: Aggiungi lattività specificata allistanza diTaskCollectionaspose.tasks/taskcollectionclass. Se ParentProject.CalculationMode è None lutente deve richiamare Project.Recalculate dopo aver utilizzato questo metodo ripianificherà tutte le attività del progetto date di inizio/fine imposta date di inizio/fine e calcolerà i campi dipendenti come slacks lavoro e campi di costo ID e livelli di struttura. Se ParentProject.CalculationMode è Manuale il metodo calcolerà automaticamente solo lID attività il livello di struttura e i numeri di struttura. Se ParentProject.CalculationMode è Automatico il metodo riprogramma automaticamente tutte le attività del progetto inizio/fine date imposta date anticipate/tardive calcola slack campi di lavoro e costi ricalcola ID e livelli di struttura.
type: docs
weight: 50
url: /it/net/aspose.tasks/taskcollection/add/
---
## Add(Task) {#add_4}

Aggiungi l'attività specificata all'istanza di[`TaskCollection`](../../taskcollection)class. Se ParentProject.CalculationMode è None l'utente deve richiamare Project.Recalculate() dopo aver utilizzato questo metodo (ripianificherà tutte le attività del progetto (date di inizio/fine, imposta date di inizio/fine) e calcolerà i campi dipendenti come slacks, lavoro e campi di costo, ID e livelli di struttura). Se ParentProject.CalculationMode è Manuale, il metodo calcolerà automaticamente solo l'ID attività, il livello di struttura e i numeri di struttura. Se ParentProject.CalculationMode è Automatico, il metodo riprogramma automaticamente tutte le attività del progetto (inizio/fine date, imposta date anticipate/tardive, calcola slack, campi di lavoro e costi, ricalcola ID e livelli di struttura).

```csharp
public void Add(Task item)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| item | Task | l'attività specificata che deve essere aggiunta a questa raccolta di attività. |

### Guarda anche

* class [Task](../../task)
* class [TaskCollection](../../taskcollection)
* spazio dei nomi [Aspose.Tasks](../../taskcollection)
* assemblea [Aspose.Tasks](../../../)

---

## Add() {#add}

Aggiunge una nuova attività alla raccolta di attività del progetto sullo stesso livello di struttura dell'ultima attività.

```csharp
public Task Add()
```

### Valore di ritorno

restituisce l'istanza appena aggiunta di[`Task`](../../task) classe.

### Guarda anche

* class [Task](../../task)
* class [TaskCollection](../../taskcollection)
* spazio dei nomi [Aspose.Tasks](../../taskcollection)
* assemblea [Aspose.Tasks](../../../)

---

## Add(string) {#add_2}

Aggiunge una nuova attività alla raccolta di attività per bambini.

```csharp
public Task Add(string taskName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| taskName | String | il nome dell'attività specificato. |

### Valore di ritorno

restituisce l'istanza appena aggiunta di[`Task`](../../task) classe.

### Guarda anche

* class [Task](../../task)
* class [TaskCollection](../../taskcollection)
* spazio dei nomi [Aspose.Tasks](../../taskcollection)
* assemblea [Aspose.Tasks](../../../)

---

## Add(string, int) {#add_3}

Aggiunge una nuova attività ricorrente alla raccolta di attività per bambini.

```csharp
public Task Add(string taskName, int beforeTaskId)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| taskName | String | il nome dell'attività specificato. |
| beforeTaskId | Int32 | L'ID specificato di un'attività prima della quale verrà inserita una nuova attività. |

### Valore di ritorno

restituisce un'attività che è stata inserita prima di un'attività con l'ID specificato.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentOutOfRangeException | Viene generata ArgumentOutOfRangeException se l'ID specificato non è un ID attività valido. |

### Guarda anche

* class [Task](../../task)
* class [TaskCollection](../../taskcollection)
* spazio dei nomi [Aspose.Tasks](../../taskcollection)
* assemblea [Aspose.Tasks](../../../)

---

## Add(RecurringTaskParameters) {#add_1}

Inserisce una nuova attività prima di un'attività con l'ID specificato e sullo stesso livello di struttura.

```csharp
public Task Add(RecurringTaskParameters parameters)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| parameters | RecurringTaskParameters | I parametri i parametri specificati per la creazione di attività ricorrenti. |

### Valore di ritorno

restituisce l'istanza appena aggiunta di[`Task`](../../task) classe.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | Generato se i parametri specificati sono null. |
| ArgumentException | Generato se i parametri specificati non sono validi. |

### Guarda anche

* class [Task](../../task)
* class [RecurringTaskParameters](../../recurringtaskparameters)
* class [TaskCollection](../../taskcollection)
* spazio dei nomi [Aspose.Tasks](../../taskcollection)
* assemblea [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
