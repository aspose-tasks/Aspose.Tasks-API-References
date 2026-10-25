---
title: "Project.SetBaseline"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo di Project. Salva i campi della baseline nella baseline specificata per l'intero progetto"
type: docs
weight: 1250
url: /it/net/aspose.tasks/project/setbaseline/
---
## SetBaseline(BaselineType) {#setbaseline}

Salva i campi di baseline nella baseline specificata per l'intero progetto.

```csharp
public void SetBaseline(BaselineType baselineType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| baselineType | BaselineType | Il tipo di baseline in cui salvare i dati della baseline. |

## Esempi

Mostra come creare baseline per un intero progetto.

```csharp
var project = new Project();

// Aggiunta di attività
project.RootTask.Children.Add("Task");
project.RootTask.Children.Add("Task2");

// Imposta baseline per le attività specificate
project.SetBaseline(BaselineType.Baseline);
```

### Vedi anche

* enum [BaselineType](../../baselinetype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SetBaseline(BaselineType, IEnumerable&lt;Task&gt;) {#setbaseline_1}

Salva i campi di baseline nella baseline specificata per le attività selezionate.

```csharp
public void SetBaseline(BaselineType baselineType, IEnumerable<Task> taskCollection)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| baselineType | BaselineType | Il tipo di baseline in cui salvare i dati della baseline. |
| taskCollection | IEnumerable`1 | Elenco di attività per le quali salvare i dati della baseline. |

## Esempi

Mostra come creare baseline impostate per attività specifiche.

```csharp
var project = new Project();

// Aggiunta di attività
var task = project.RootTask.Children.Add("Task");
var task2 = project.RootTask.Children.Add("Task2");

// Imposta baseline per le attività specificate
project.SetBaseline(BaselineType.Baseline, new[] { task, task2 });
```

### Vedi anche

* enum [BaselineType](../../baselinetype/)
* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


