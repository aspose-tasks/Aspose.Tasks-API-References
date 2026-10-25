---
title: "Aspose::Tasks::TaskLinkCollection::Add метод"
linktitle: "Add"
articleTitle: "Add"
second_title: "Aspose.Tasks для C++"
description: "Возвращает экземпляр связи Finish-Start TaskLink, который был добавлен в объект TaskLinkCollection."
type: docs
weight: 10
url: /ru/cpp/aspose.tasks/tasklinkcollection/add/
---

## Add (1 of 4) {#add_1}

Возвращает экземпляр связи Finish-Start TaskLink, который был добавлен в объект TaskLinkCollection.

**Returns:** a task link instance which has been added to this object.

```cpp
Add(const System::SharedPtr< Task > & pred, const System::SharedPtr< Task > & succ)
```

| Параметр | Описание |
| --- | --- |
| pred | Предшествующая задача. |
| succ | Последующая задача. |

---

## Add (2 of 4) {#add_2}

Возвращает экземпляр TaskLink, который был добавлен в объект TaskLinkCollection.

**Returns:** a task link instance which has been added to this object.

```cpp
Add(const System::SharedPtr< Task > & pred, const System::SharedPtr< Task > & succ, TaskLinkType linkType)
```

| Параметр | Описание |
| --- | --- |
| pred | Предшествующая задача. |
| succ | Последующая задача. |
| linkType | Тип ссылки TaskLinkType |

---

## Add (3 of 4) {#add_3}

Возвращает экземпляр TaskLink, который был добавлен в объект TaskLinkCollection.

**Returns:** a task link which has been added to this object.

```cpp
Add(const System::SharedPtr< Task > & pred, const System::SharedPtr< Task > & succ, TaskLinkType linkType, Duration lag)
```

| Параметр | Описание |
| --- | --- |
| pred | Предшествующая задача. |
| succ | Последующая задача. |
| linkType | Тип ссылки TaskLinkType |
| lag | Задержка связи Duration. |

---

## Add (4 of 4) {#add_4}

Это заглушка реализации метода Add интерфейса ICollection, который только бросает NotSupportedException

**Returns:** void Aspose::Tasks::

```cpp
Add(const System::SharedPtr< TaskLink > & item)
```

| Параметр | Описание |
| --- | --- |
| элемент | Элемент для добавления. |

