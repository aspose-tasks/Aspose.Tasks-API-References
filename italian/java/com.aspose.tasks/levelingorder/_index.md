---
title: "LevelingOrder"
second_title: "Aspose.Tasks for Java API Reference"
description: "Definisce i possibili valori dell'ordine di livellamento."
type: docs
weight: 143
url: /it/java/com.aspose.tasks/levelingorder/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class LevelingOrder extends System.Enum
```

Definisce i possibili valori dell'ordine di livellamento.
## Campi

| Campo | Descrizione |
| --- | --- |
| [IdOnly](#IdOnly) | Le attività sono ritardate in ordine crescente di Id. |
| [PriorityThenStandard](#PriorityThenStandard) | La priorità è considerata per prima, poi le stesse proprietà di Standard. |
| [Standard](#Standard) | Le seguenti proprietà sono prese in considerazione: relazioni di predecessore, margine totale (un'attività con margine totale più alto è ritardata per prima), data di inizio, priorità. |
### IdOnly {#IdOnly}
```
public static final int IdOnly
```


Le attività sono ritardate in ordine crescente di Id.

### PriorityThenStandard {#PriorityThenStandard}
```
public static final int PriorityThenStandard
```


La priorità è considerata per prima, poi le stesse proprietà di Standard.

### Standard {#Standard}
```
public static final int Standard
```


Le seguenti proprietà sono prese in considerazione: relazioni di predecessore, margine totale (un'attività con margine totale più alto è ritardata per prima), data di inizio, priorità. Questo è il valore predefinito.

