---
title: "Aspose::Tasks::TaskLinkCollection::Add metodo"
linktitle: "Add"
articleTitle: "Add"
second_title: "Aspose.Tasks per C++"
description: "Restituisce un'istanza di TaskLink Finish-Start che è stata aggiunta all'oggetto TaskLinkCollection."
type: docs
weight: 10
url: /it/cpp/aspose.tasks/tasklinkcollection/add/
---

## Add (1 of 4) {#add_1}

Restituisce un'istanza di TaskLink Finish-Start che è stata aggiunta all'oggetto TaskLinkCollection.

**Returns:** a task link instance which has been added to this object.

```cpp
Add(const System::SharedPtr< Task > & pred, const System::SharedPtr< Task > & succ)
```

| Parametro | Descrizione |
| --- | --- |
| pred | Attività predecessore. |
| succ | Attività successore. |

---

## Add (2 of 4) {#add_2}

Restituisce un'istanza di TaskLink che è stata aggiunta all'oggetto TaskLinkCollection.

**Returns:** a task link instance which has been added to this object.

```cpp
Add(const System::SharedPtr< Task > & pred, const System::SharedPtr< Task > & succ, TaskLinkType linkType)
```

| Parametro | Descrizione |
| --- | --- |
| pred | Attività predecessore. |
| succ | Attività successore. |
| linkType | Tipo di collegamento TaskLinkType |

---

## Add (3 of 4) {#add_3}

Restituisce un'istanza di TaskLink che è stata aggiunta all'oggetto TaskLinkCollection.

**Returns:** a task link which has been added to this object.

```cpp
Add(const System::SharedPtr< Task > & pred, const System::SharedPtr< Task > & succ, TaskLinkType linkType, Duration lag)
```

| Parametro | Descrizione |
| --- | --- |
| pred | Attività predecessore. |
| succ | Attività successore. |
| linkType | Tipo di collegamento TaskLinkType |
| lag | Durata del ritardo del collegamento. |

---

## Add (4 of 4) {#add_4}

Questa è l'implementazione stub del metodo Add di ICollection, che lancia solo NotSupportedException

**Returns:** void Aspose::Tasks::

```cpp
Add(const System::SharedPtr< TaskLink > & item)
```

| Parametro | Descrizione |
| --- | --- |
| elemento | L'elemento da aggiungere. |

