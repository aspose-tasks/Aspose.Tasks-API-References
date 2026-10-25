---
title: "Aspose::Tasks::TaskLinkCollection::Add μέθοδος"
linktitle: "Προσθήκη"
articleTitle: "Προσθήκη"
second_title: "Aspose.Tasks για C++"
description: "Επιστρέφει ένα στιγμιότυπο του TaskLink Finish-Start που έχει προστεθεί στο αντικείμενο TaskLinkCollection."
type: docs
weight: 10
url: /el/cpp/aspose.tasks/tasklinkcollection/add/
---

## Add (1 of 4) {#add_1}

Επιστρέφει ένα στιγμιότυπο του TaskLink Finish-Start που έχει προστεθεί στο αντικείμενο TaskLinkCollection.

**Returns:** a task link instance which has been added to this object.

```cpp
Add(const System::SharedPtr< Task > & pred, const System::SharedPtr< Task > & succ)
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| pred | Προηγούμενη εργασία. |
| succ | Επόμενη εργασία. |

---

## Add (2 of 4) {#add_2}

Επιστρέφει ένα αντικείμενο TaskLink που έχει προστεθεί στο αντικείμενο TaskLinkCollection.

**Returns:** a task link instance which has been added to this object.

```cpp
Add(const System::SharedPtr< Task > & pred, const System::SharedPtr< Task > & succ, TaskLinkType linkType)
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| pred | Προηγούμενη εργασία. |
| succ | Επόμενη εργασία. |
| linkType | Τύπος σύνδεσης TaskLinkType |

---

## Add (3 of 4) {#add_3}

Επιστρέφει ένα αντικείμενο TaskLink που έχει προστεθεί στο αντικείμενο TaskLinkCollection.

**Returns:** a task link which has been added to this object.

```cpp
Add(const System::SharedPtr< Task > & pred, const System::SharedPtr< Task > & succ, TaskLinkType linkType, Duration lag)
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| pred | Προηγούμενη εργασία. |
| succ | Επόμενη εργασία. |
| linkType | Τύπος σύνδεσης TaskLinkType |
| lag | Καθυστέρηση σύνδεσης Duration . |

---

## Add (4 of 4) {#add_4}

Αυτή είναι η ψευδο-εφαρμογή της μεθόδου Add του ICollection, η οποία μόνο ρίχνει NotSupportedException.

**Returns:** void Aspose::Tasks::

```cpp
Add(const System::SharedPtr< TaskLink > & item)
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| αντικείμενο | Το στοιχείο για προσθήκη. |

