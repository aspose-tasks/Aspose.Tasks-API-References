---
title: "Aspose::Tasks::TaskLinkCollection::Add method"
linktitle: "Add"
articleTitle: "Add"
second_title: "Aspose.Tasks für C++"
description: "Gibt eine Instanz eines Finish-Start TaskLink zurück, die dem TaskLinkCollection-Objekt hinzugefügt wurde."
type: docs
weight: 10
url: /de/cpp/aspose.tasks/tasklinkcollection/add/
---

## Add (1 of 4) {#add_1}

Gibt eine Instanz eines Finish-Start TaskLink zurück, die dem TaskLinkCollection-Objekt hinzugefügt wurde.

**Returns:** a task link instance which has been added to this object.

```cpp
Add(const System::SharedPtr< Task > & pred, const System::SharedPtr< Task > & succ)
```

| Parameter | Beschreibung |
| --- | --- |
| pred | Vorgängeraufgabe. |
| succ | Nachfolgeraufgabe. |

---

## Add (2 of 4) {#add_2}

Gibt eine Instanz von TaskLink zurück, die dem TaskLinkCollection-Objekt hinzugefügt wurde.

**Returns:** a task link instance which has been added to this object.

```cpp
Add(const System::SharedPtr< Task > & pred, const System::SharedPtr< Task > & succ, TaskLinkType linkType)
```

| Parameter | Beschreibung |
| --- | --- |
| pred | Vorgängeraufgabe. |
| succ | Nachfolgeraufgabe. |
| linkType | Linktyp TaskLinkType |

---

## Add (3 of 4) {#add_3}

Gibt eine Instanz von TaskLink zurück, die dem TaskLinkCollection-Objekt hinzugefügt wurde.

**Returns:** a task link which has been added to this object.

```cpp
Add(const System::SharedPtr< Task > & pred, const System::SharedPtr< Task > & succ, TaskLinkType linkType, Duration lag)
```

| Parameter | Beschreibung |
| --- | --- |
| pred | Vorgängeraufgabe. |
| succ | Nachfolgeraufgabe. |
| linkType | Linktyp TaskLinkType |
| lag | Link-Latenzdauer. |

---

## Add (4 of 4) {#add_4}

Dies ist die Stub-Implementierung der Add-Methode von ICollection, die nur NotSupportedException wirft.

**Returns:** void Aspose::Tasks::

```cpp
Add(const System::SharedPtr< TaskLink > & item)
```

| Parameter | Beschreibung |
| --- | --- |
| Element | Das hinzuzufügende Element. |

