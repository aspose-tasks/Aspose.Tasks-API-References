---
title: WorkingTime.WorkingTime
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: WorkingTime costruttore. Inizializza una nuova istanza diWorkingTime classe con un intervallo con gli orari di inizio e fine specificati.
type: docs
weight: 10
url: /it/net/aspose.tasks/workingtime/workingtime/
---
## WorkingTime(DateTime, DateTime) {#constructor_1}

Inizializza una nuova istanza di[`WorkingTime`](../) classe con un intervallo con gli orari di inizio e fine specificati.

```csharp
public WorkingTime(DateTime fromTime, DateTime toTime)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fromTime | DateTime | ora di inizio dell'intervallo |
| toTime | DateTime | ora di fine intervallo |

### Guarda anche

* class [WorkingTime](../)
* spazio dei nomi [Aspose.Tasks](../../workingtime/)
* assemblea [Aspose.Tasks](../../../)

---

## WorkingTime(TimeSpan, TimeSpan) {#constructor_2}

Inizializza una nuova istanza di[`WorkingTime`](../) classe con un elemento intervallo con gli orari di inizio e fine specificati.

```csharp
public WorkingTime(TimeSpan fromTime, TimeSpan toTime)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fromTime | TimeSpan | L'ora di inizio dell'intervallo rappresentata daTimeSpan struct. |
| toTime | TimeSpan | L'ora di fine dell'intervallo rappresentata daTimeSpan struct. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentException | Quando toTime minore di uguale a toTime argomento o quando l'intervallo tra fromTime e toTime è maggiore di 24 ore. |

### Esempi

L'overload di WorkingTime ctor può essere utilizzato per inizializzare l'inizio e la fine dell'intervallo utilizzando TimeSpans:

```csharp
[C#]
var wt = new WorkingTime(new TimeSpan(9, 0, 0), new TimeSpan(18, 0, 0));
```

### Guarda anche

* class [WorkingTime](../)
* spazio dei nomi [Aspose.Tasks](../../workingtime/)
* assemblea [Aspose.Tasks](../../../)

---

## WorkingTime(int, int) {#constructor}

Inizializza una nuova istanza di[`WorkingTime`](../) classe con un elemento intervallo con gli orari di inizio e fine specificati.

```csharp
public WorkingTime(int fromHours, int toHours)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fromHours | Int32 | L'ora di inizio dell'intervallo rappresentata dal numero intero di ore (0-24). |
| toHours | Int32 | L'ora di fine dell'intervallo rappresentata dal numero intero di ore (0-24). |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentException | Quando toTime minore di uguale a toTime argomento o quando l'intervallo tra fromTime e toTime è maggiore di 24 ore. |

### Esempi

L'overload di WorkingTime ctor può essere utilizzato per inizializzare l'inizio e la fine dell'intervallo utilizzando ore intere:

```csharp
[C#]
var wt = new WorkingTime(9, 13);
```

### Guarda anche

* class [WorkingTime](../)
* spazio dei nomi [Aspose.Tasks](../../workingtime/)
* assemblea [Aspose.Tasks](../../../)


