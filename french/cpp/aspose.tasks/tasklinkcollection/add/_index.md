---
title: "Aspose::Tasks::TaskLinkCollection::Add méthode"
linktitle: "Ajouter"
articleTitle: "Ajouter"
second_title: "Aspose.Tasks pour C++"
description: "Renvoie une instance de TaskLink Finish-Start qui a été ajoutée à l'objet TaskLinkCollection."
type: docs
weight: 10
url: /fr/cpp/aspose.tasks/tasklinkcollection/add/
---

## Add (1 of 4) {#add_1}

Renvoie une instance de TaskLink Finish-Start qui a été ajoutée à l'objet TaskLinkCollection.

**Returns:** a task link instance which has been added to this object.

```cpp
Add(const System::SharedPtr< Task > & pred, const System::SharedPtr< Task > & succ)
```

| Paramètre | Description |
| --- | --- |
| pred | Tâche prédécesseur. |
| succ | Tâche successeur. |

---

## Add (2 of 4) {#add_2}

Renvoie une instance de TaskLink qui a été ajoutée à l'objet TaskLinkCollection.

**Returns:** a task link instance which has been added to this object.

```cpp
Add(const System::SharedPtr< Task > & pred, const System::SharedPtr< Task > & succ, TaskLinkType linkType)
```

| Paramètre | Description |
| --- | --- |
| pred | Tâche prédécesseur. |
| succ | Tâche successeur. |
| linkType | Type de lien TaskLinkType |

---

## Add (3 of 4) {#add_3}

Renvoie une instance de TaskLink qui a été ajoutée à l'objet TaskLinkCollection.

**Returns:** a task link which has been added to this object.

```cpp
Add(const System::SharedPtr< Task > & pred, const System::SharedPtr< Task > & succ, TaskLinkType linkType, Duration lag)
```

| Paramètre | Description |
| --- | --- |
| pred | Tâche prédécesseur. |
| succ | Tâche successeur. |
| linkType | Type de lien TaskLinkType |
| lag | Durée du retard du lien. |

---

## Add (4 of 4) {#add_4}

Ceci est l'implémentation factice de la méthode Add de ICollection, qui ne fait que lever NotSupportedException.

**Returns:** void Aspose::Tasks::

```cpp
Add(const System::SharedPtr< TaskLink > & item)
```

| Paramètre | Description |
| --- | --- |
| élément | L'élément à ajouter. |

