---
title: "Aspose::Tasks::ResourceAssignmentCollection::Add método"
linktitle: "Add"
articleTitle: "Add"
second_title: "Aspose.Tasks for C++"
description: "Esta es la implementación de sustituto del método Add de ICollection, que solo lanza NotSupportedException"
type: docs
weight: 10
url: /es/cpp/aspose.tasks/resourceassignmentcollection/add/
---

## Add (1 of 4) {#add_1}

Esta es la implementación de sustituto del método Add de ICollection, que solo lanza NotSupportedException

**Returns:** void Aspose::Tasks::

```cpp
Add(const System::SharedPtr< ResourceAssignment > & item)
```

| Parámetro | Descripción |
| --- | --- |
| elemento | El elemento a eliminar. |

---

## Add (2 of 4) {#add_2}

Agrega una nueva asignación a la ResourceAssignmentCollection.

**Returns:** Added assignment.

```cpp
Add(const System::SharedPtr< Task > & task, const System::SharedPtr< Resource > & resource)
```

| Parámetro | Descripción |
| --- | --- |
| tarea | Una tarea para asignar. |
| recurso | Un recurso para asignar. |

---

## Add (3 of 4) {#add_3}

Agrega una nueva asignación a la ResourceAssignmentCollection.

**Returns:** Added assignment.

```cpp
Add(const System::SharedPtr< Task > & task, const System::SharedPtr< Resource > & resource, double units)
```

| Parámetro | Descripción |
| --- | --- |
| tarea | Una tarea para asignar. |
| recurso | Un recurso para asignar. |
| unidades | El número de unidades para una nueva asignación. |

---

## Add (4 of 4) {#add_4}

Agrega una nueva asignación a la ResourceAssignmentCollection.

**Returns:** Added assignment.

```cpp
Add(const System::SharedPtr< Task > & task, const System::SharedPtr< Resource > & resource, System::Decimal cost)
```

| Parámetro | Descripción |
| --- | --- |
| tarea | Una tarea para asignar. |
| recurso | Un recurso de costo para asignar. |
| costo | El costo para una nueva asignación. |

