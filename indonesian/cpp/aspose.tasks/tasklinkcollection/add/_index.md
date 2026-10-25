---
title: "Aspose::Tasks::TaskLinkCollection::Add metode"
linktitle: "Add"
articleTitle: "Add"
second_title: "Aspose.Tasks untuk C++"
description: "Mengembalikan instance dari Finish-Start TaskLink yang telah ditambahkan ke objek TaskLinkCollection."
type: docs
weight: 10
url: /id/cpp/aspose.tasks/tasklinkcollection/add/
---

## Add (1 of 4) {#add_1}

Mengembalikan instance dari Finish-Start TaskLink yang telah ditambahkan ke objek TaskLinkCollection.

**Returns:** a task link instance which has been added to this object.

```cpp
Add(const System::SharedPtr< Task > & pred, const System::SharedPtr< Task > & succ)
```

| Parameter | Deskripsi |
| --- | --- |
| pred | Tugas pendahulu. |
| succ | Tugas penerus. |

---

## Add (2 of 4) {#add_2}

Mengembalikan sebuah instance dari TaskLink yang telah ditambahkan ke objek TaskLinkCollection.

**Returns:** a task link instance which has been added to this object.

```cpp
Add(const System::SharedPtr< Task > & pred, const System::SharedPtr< Task > & succ, TaskLinkType linkType)
```

| Parameter | Deskripsi |
| --- | --- |
| pred | Tugas pendahulu. |
| succ | Tugas penerus. |
| linkType | Tipe tautan TaskLinkType |

---

## Add (3 of 4) {#add_3}

Mengembalikan sebuah instance dari TaskLink yang telah ditambahkan ke objek TaskLinkCollection.

**Returns:** a task link which has been added to this object.

```cpp
Add(const System::SharedPtr< Task > & pred, const System::SharedPtr< Task > & succ, TaskLinkType linkType, Duration lag)
```

| Parameter | Deskripsi |
| --- | --- |
| pred | Tugas pendahulu. |
| succ | Tugas penerus. |
| linkType | Tipe tautan TaskLinkType |
| lag | Durasi jeda tautan. |

---

## Add (4 of 4) {#add_4}

Ini adalah implementasi stub dari metode Add milik ICollection, yang hanya melempar NotSupportedException

**Returns:** void Aspose::Tasks::

```cpp
Add(const System::SharedPtr< TaskLink > & item)
```

| Parameter | Deskripsi |
| --- | --- |
| item | Item yang akan ditambahkan. |

