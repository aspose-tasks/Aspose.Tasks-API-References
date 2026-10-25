---
title: "SimpleSaveOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "Questa è una classe base astratta che consente all'utente di specificare opzioni di base durante il salvataggio di un progetto in un formato specifico."
type: docs
weight: 277
url: /it/java/com.aspose.tasks/simplesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public abstract class SimpleSaveOptions
```

Questa è una classe base astratta che consente all'utente di specificare opzioni di base durante il salvataggio di un progetto in un formato specifico.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [SimpleSaveOptions()](#SimpleSaveOptions--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getSaveFormat()](#getSaveFormat--) | Ottiene il formato in cui il documento verrà salvato se viene utilizzato questo oggetto di opzioni di salvataggio. |
| [getTasksComparer()](#getTasksComparer--) | Ottiene il comparatore per ordinare le attività nel diagramma di Gantt e nel diagramma Foglio attività. |
| [getTasksFilter()](#getTasksFilter--) | Ottiene la condizione utilizzata per filtrare le attività visualizzate nei diagrammi Gantt, Foglio attività e Utilizzo attività. |
| [setTasksComparer(Comparator&lt;Task&gt; value)](#setTasksComparer-java.util.Comparator-com.aspose.tasks.Task--) | Imposta il comparatore per ordinare le attività nel diagramma di Gantt e nel diagramma Foglio attività. |
| [setTasksFilter(ICondition&lt;Task&gt; value)](#setTasksFilter-com.aspose.tasks.ICondition-com.aspose.tasks.Task--) | Imposta la condizione utilizzata per filtrare le attività visualizzate nei diagrammi Gantt, Foglio attività e Utilizzo attività. |
### SimpleSaveOptions() {#SimpleSaveOptions--}
```
public SimpleSaveOptions()
```


### getSaveFormat() {#getSaveFormat--}
```
public final int getSaveFormat()
```


Ottiene il formato in cui il documento verrà salvato se viene utilizzato questo oggetto di opzioni di salvataggio.

**Returns:**
int - il [SaveFileFormat](../../com.aspose.tasks/savefileformat) in cui il documento verrà salvato.
### getTasksComparer() {#getTasksComparer--}
```
public final Comparator<Task> getTasksComparer()
```


Ottiene il comparatore per ordinare le attività nel diagramma di Gantt e nel diagramma Foglio attività.

**Returns:**
java.util.Comparator&lt;com.aspose.tasks.Task&gt; - il comparatore per ordinare le attività nel diagramma di Gantt e nel diagramma Foglio attività.
### getTasksFilter() {#getTasksFilter--}
```
public final ICondition<Task> getTasksFilter()
```


Ottiene la condizione utilizzata per filtrare le attività visualizzate nei diagrammi Gantt, Foglio attività e Utilizzo attività.

--------------------

Se il valore non è specificato, viene utilizzato il filtro predefinito che rimuove le attività non visibili -- cioè le attività discendenti di attività compresse.

**Returns:**
[ICondition](../../com.aspose.tasks/icondition) - the condition which is used to filter tasks rendered on Gantt, Task Sheet and Task Usage charts.
### setTasksComparer(Comparator&lt;Task&gt; value) {#setTasksComparer-java.util.Comparator-com.aspose.tasks.Task--}
```
public final void setTasksComparer(Comparator<Task> value)
```


Imposta il comparatore per ordinare le attività nel diagramma di Gantt e nel diagramma Foglio attività.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Comparator&lt;com.aspose.tasks.Task&gt; | il comparatore per ordinare le attività nel diagramma di Gantt e nel diagramma Foglio attività. |

### setTasksFilter(ICondition&lt;Task&gt; value) {#setTasksFilter-com.aspose.tasks.ICondition-com.aspose.tasks.Task--}
```
public final void setTasksFilter(ICondition<Task> value)
```


Imposta la condizione utilizzata per filtrare le attività visualizzate nei diagrammi Gantt, Foglio attività e Utilizzo attività.

--------------------

Se il valore non è specificato, viene utilizzato il filtro predefinito che rimuove le attività non visibili -- cioè le attività discendenti di attività compresse.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | com.aspose.tasks.ICondition&lt;com.aspose.tasks.Task&gt; | la condizione utilizzata per filtrare le attività visualizzate su diagrammi Gantt, Foglio attività e Utilizzo attività. |

