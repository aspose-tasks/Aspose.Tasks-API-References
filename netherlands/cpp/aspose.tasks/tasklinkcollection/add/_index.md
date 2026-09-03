---
title: "Aspose::Tasks::TaskLinkCollection::Add methode"
linktitle: "Toevoegen"
articleTitle: "Toevoegen"
second_title: "Aspose.Tasks voor C++"
description: "Retourneert een exemplaar van Finish-Start TaskLink dat is toegevoegd aan het TaskLinkCollection-object."
type: docs
weight: 10
url: /nl/cpp/aspose.tasks/tasklinkcollection/add/
---

## Add (1 of 4) {#add_1}

Retourneert een exemplaar van Finish-Start TaskLink dat is toegevoegd aan het TaskLinkCollection-object.

**Returns:** a task link instance which has been added to this object.

```cpp
Add(const System::SharedPtr< Task > & pred, const System::SharedPtr< Task > & succ)
```

| Parameter | Beschrijving |
| --- | --- |
| pred | Voorgaande taak. |
| succ | Opvolgende taak. |

---

## Add (2 of 4) {#add_2}

Retourneert een instantie van TaskLink die is toegevoegd aan het TaskLinkCollection-object.

**Returns:** a task link instance which has been added to this object.

```cpp
Add(const System::SharedPtr< Task > & pred, const System::SharedPtr< Task > & succ, TaskLinkType linkType)
```

| Parameter | Beschrijving |
| --- | --- |
| pred | Voorgaande taak. |
| succ | Opvolgende taak. |
| linkType | Koppelingstype TaskLinkType |

---

## Add (3 of 4) {#add_3}

Retourneert een instantie van TaskLink die is toegevoegd aan het TaskLinkCollection-object.

**Returns:** a task link which has been added to this object.

```cpp
Add(const System::SharedPtr< Task > & pred, const System::SharedPtr< Task > & succ, TaskLinkType linkType, Duration lag)
```

| Parameter | Beschrijving |
| --- | --- |
| pred | Voorgaande taak. |
| succ | Opvolgende taak. |
| linkType | Koppelingstype TaskLinkType |
| lag | Koppeling vertraging Duur . |

---

## Add (4 of 4) {#add_4}

Dit is de stub-implementatie van de Add-methode van ICollection, die alleen een NotSupportedException gooit.

**Returns:** void Aspose::Tasks::

```cpp
Add(const System::SharedPtr< TaskLink > & item)
```

| Parameter | Beschrijving |
| --- | --- |
| item | Het item om toe te voegen. |

