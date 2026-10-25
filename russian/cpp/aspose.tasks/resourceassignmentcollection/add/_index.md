---
title: "Aspose::Tasks::ResourceAssignmentCollection::Add метод"
linktitle: "Add"
articleTitle: "Add"
second_title: "Aspose.Tasks для C++"
description: "Это заглушка реализации метода Add интерфейса ICollection, который только бросает NotSupportedException"
type: docs
weight: 10
url: /ru/cpp/aspose.tasks/resourceassignmentcollection/add/
---

## Add (1 of 4) {#add_1}

Это заглушка реализации метода Add интерфейса ICollection, который только бросает NotSupportedException

**Returns:** void Aspose::Tasks::

```cpp
Add(const System::SharedPtr< ResourceAssignment > & item)
```

| Параметр | Описание |
| --- | --- |
| элемент | Элемент для удаления. |

---

## Add (2 of 4) {#add_2}

Добавляет новое назначение в ResourceAssignmentCollection .

**Returns:** Added assignment.

```cpp
Add(const System::SharedPtr< Task > & task, const System::SharedPtr< Resource > & resource)
```

| Параметр | Описание |
| --- | --- |
| задача | Задача для назначения. |
| ресурс | Ресурс для назначения. |

---

## Add (3 of 4) {#add_3}

Добавляет новое назначение в ResourceAssignmentCollection .

**Returns:** Added assignment.

```cpp
Add(const System::SharedPtr< Task > & task, const System::SharedPtr< Resource > & resource, double units)
```

| Параметр | Описание |
| --- | --- |
| задача | Задача для назначения. |
| ресурс | Ресурс для назначения. |
| единицы | Количество единиц для нового назначения. |

---

## Add (4 of 4) {#add_4}

Добавляет новое назначение в ResourceAssignmentCollection .

**Returns:** Added assignment.

```cpp
Add(const System::SharedPtr< Task > & task, const System::SharedPtr< Resource > & resource, System::Decimal cost)
```

| Параметр | Описание |
| --- | --- |
| задача | Задача для назначения. |
| ресурс | Ресурс стоимости, который будет назначен. |
| стоимость | Стоимость нового назначения. |

