---
title: "Aspose::Tasks::TaskLinkCollection::Add método"
linktitle: "Add"
articleTitle: "Add"
second_title: "Aspose.Tasks for C++"
description: "Devuelve una instancia de TaskLink Finish-Start que ha sido añadida al objeto TaskLinkCollection."
type: docs
weight: 10
url: /es/cpp/aspose.tasks/tasklinkcollection/add/
---

## Add (1 of 4) {#add_1}

Devuelve una instancia de TaskLink Finish-Start que ha sido añadida al objeto TaskLinkCollection.

**Returns:** a task link instance which has been added to this object.

```cpp
Add(const System::SharedPtr< Task > & pred, const System::SharedPtr< Task > & succ)
```

| Parámetro | Descripción |
| --- | --- |
| pred | Tarea predecesora. |
| succ | Tarea sucesora. |

---

## Add (2 of 4) {#add_2}

Devuelve una instancia de TaskLink que ha sido añadida al objeto TaskLinkCollection.

**Returns:** a task link instance which has been added to this object.

```cpp
Add(const System::SharedPtr< Task > & pred, const System::SharedPtr< Task > & succ, TaskLinkType linkType)
```

| Parámetro | Descripción |
| --- | --- |
| pred | Tarea predecesora. |
| succ | Tarea sucesora. |
| linkType | Tipo de enlace TaskLinkType |

---

## Add (3 of 4) {#add_3}

Devuelve una instancia de TaskLink que ha sido añadida al objeto TaskLinkCollection.

**Returns:** a task link which has been added to this object.

```cpp
Add(const System::SharedPtr< Task > & pred, const System::SharedPtr< Task > & succ, TaskLinkType linkType, Duration lag)
```

| Parámetro | Descripción |
| --- | --- |
| pred | Tarea predecesora. |
| succ | Tarea sucesora. |
| linkType | Tipo de enlace TaskLinkType |
| lag | Duración del retraso del enlace. |

---

## Add (4 of 4) {#add_4}

Esta es la implementación de sustituto del método Add de ICollection, que solo lanza NotSupportedException

**Returns:** void Aspose::Tasks::

```cpp
Add(const System::SharedPtr< TaskLink > & item)
```

| Parámetro | Descripción |
| --- | --- |
| elemento | El elemento a añadir. |

