---
title: "Aspose::Tasks::TaskLinkCollection::Add metodu"
linktitle: "Ekle"
articleTitle: "Ekle"
second_title: "C++ için Aspose.Tasks"
description: "TaskLinkCollection nesnesine eklenmiş Finish-Start TaskLink örneğini döndürür."
type: docs
weight: 10
url: /tr/cpp/aspose.tasks/tasklinkcollection/add/
---

## Add (1 of 4) {#add_1}

TaskLinkCollection nesnesine eklenmiş Finish-Start TaskLink örneğini döndürür.

**Returns:** a task link instance which has been added to this object.

```cpp
Add(const System::SharedPtr< Task > & pred, const System::SharedPtr< Task > & succ)
```

| Parametre | Açıklama |
| --- | --- |
| pred | Önceki görev. |
| succ | Sonraki görev. |

---

## Add (2 of 4) {#add_2}

TaskLinkCollection nesnesine eklenmiş bir TaskLink örneğini döndürür.

**Returns:** a task link instance which has been added to this object.

```cpp
Add(const System::SharedPtr< Task > & pred, const System::SharedPtr< Task > & succ, TaskLinkType linkType)
```

| Parametre | Açıklama |
| --- | --- |
| pred | Önceki görev. |
| succ | Sonraki görev. |
| linkType | Bağlantı türü TaskLinkType |

---

## Add (3 of 4) {#add_3}

TaskLinkCollection nesnesine eklenmiş bir TaskLink örneğini döndürür.

**Returns:** a task link which has been added to this object.

```cpp
Add(const System::SharedPtr< Task > & pred, const System::SharedPtr< Task > & succ, TaskLinkType linkType, Duration lag)
```

| Parametre | Açıklama |
| --- | --- |
| pred | Önceki görev. |
| succ | Sonraki görev. |
| linkType | Bağlantı türü TaskLinkType |
| lag | Bağlantı gecikme Süresi. |

---

## Add (4 of 4) {#add_4}

Bu, ICollection'ın Add metodunun sadece NotSupportedException fırlattığı stub uygulamasıdır.

**Returns:** void Aspose::Tasks::

```cpp
Add(const System::SharedPtr< TaskLink > & item)
```

| Parametre | Açıklama |
| --- | --- |
| öğe | Eklenecek öğe. |

