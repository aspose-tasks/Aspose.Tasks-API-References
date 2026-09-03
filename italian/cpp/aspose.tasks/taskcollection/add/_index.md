---
title: "Aspose::Tasks::TaskCollection::Add metodo"
linktitle: "Add"
articleTitle: "Add"
second_title: "Aspose.Tasks per C++"
description: "Aggiunge un nuovo task alla raccolta di task del progetto allo stesso livello di outline dell'ultimo task."
type: docs
weight: 10
url: /it/cpp/aspose.tasks/taskcollection/add/
---

## Add (1 of 5) {#add_1}

Aggiunge un nuovo task alla raccolta di task del progetto allo stesso livello di outline dell'ultimo task.

**Returns:** returns the newly added instance of the Task class.

```cpp
Add()
```

---

## Add (2 of 5) {#add_2}

Inserisce una nuova attività prima di un'attività con l'ID specificato e allo stesso livello di struttura.

**Returns:** returns the newly added instance of the Task class.

```cpp
Add(const System::SharedPtr< RecurringTaskParameters > & parameters)
```

| Parametro | Descrizione |
| --- | --- |
| parametri | I parametri specificati per la creazione di un'attività ricorrente. |

---

## Add (3 of 5) {#add_3}

Aggiungi l'attività specificata all'istanza della classe TaskCollection. Se ParentProject.CalculationMode è None l'utente dovrebbe invocare Project.Recalculate() dopo aver usato questo metodo (Riprogrammerà tutte le attività del progetto (date di inizio/fine, imposta le date anticipate/posticipate) e calcolerà i campi dipendenti come ritardi, lavoro e costi, ID e livelli di struttura). Se ParentProject.CalculationMode è Manual il metodo calcolerà solo l'ID dell'attività, il livello di struttura e i numeri di struttura automaticamente. Se ParentProject.CalculationMode è Automatic il metodo riprogramma automaticamente tutte le attività del progetto (date di inizio/fine, imposta le date anticipate/posticipate, calcola i ritardi, lavoro e costi, ricalcola ID e livelli di struttura).

**Returns:** void Aspose::Tasks::

```cpp
Add(const System::SharedPtr< Task > & item)
```

| Parametro | Descrizione |
| --- | --- |
| elemento | l'attività specificata che dovrebbe essere aggiunta a questa raccolta di attività. |

---

## Add (4 of 5) {#add_4}

Aggiunge una nuova attività alla raccolta di attività figlie.

**Returns:** returns the newly added instance of the Task class.

```cpp
Add(const System::String & taskName)
```

| Parametro | Descrizione |
| --- | --- |
| taskName | il nome dell'attività specificata. |

---

## Add (5 of 5) {#add_5}

Aggiunge una nuova attività ricorrente alla raccolta di attività figlie.

**Returns:** returns a task which was inserted before a task with the specified id.

```cpp
Add(const System::String & taskName, int32_t beforeTaskId)
```

| Parametro | Descrizione |
| --- | --- |
| taskName | il nome dell'attività specificata. |
| beforeTaskId | L'ID specificato di un'attività prima della quale verrà inserita una nuova attività. |

