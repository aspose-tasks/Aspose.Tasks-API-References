---
title: "Aspose::Tasks::TaskCollection::Add método"
linktitle: "Add"
articleTitle: "Add"
second_title: "Aspose.Tasks for C++"
description: "Agrega una nueva tarea a la colección de tareas del proyecto en el mismo nivel de esquema que la última tarea."
type: docs
weight: 10
url: /es/cpp/aspose.tasks/taskcollection/add/
---

## Add (1 of 5) {#add_1}

Agrega una nueva tarea a la colección de tareas del proyecto en el mismo nivel de esquema que la última tarea.

**Returns:** returns the newly added instance of the Task class.

```cpp
Add()
```

---

## Add (2 of 5) {#add_2}

Inserta una nueva tarea antes de una tarea con el id especificado y en el mismo nivel de esquema.

**Returns:** returns the newly added instance of the Task class.

```cpp
Add(const System::SharedPtr< RecurringTaskParameters > & parameters)
```

| Parámetro | Descripción |
| --- | --- |
| parámetros | Los parámetros especificados para la creación de una tarea recurrente. |

---

## Add (3 of 5) {#add_3}

Agrega la tarea especificada a la instancia de la clase TaskCollection. Si ParentProject.CalculationMode es None, el usuario debe invocar Project.Recalculate() después de usar este método (Reprogramará todas las tareas del proyecto (fechas de inicio/fin, establece fechas tempranas/tardías) y calculará los campos dependientes como holguras, trabajo y campos de costo, identificadores y niveles de esquema). Si ParentProject.CalculationMode es Manual, el método calculará solo el id de la tarea, el nivel de esquema y los números de esquema automáticamente. Si ParentProject.CalculationMode es Automatic, el método reprograma automáticamente todas las tareas del proyecto (fechas de inicio/fin, establece fechas tempranas/tardías, calcula holguras, trabajo y campos de costo, recalcula identificadores y niveles de esquema).

**Returns:** void Aspose::Tasks::

```cpp
Add(const System::SharedPtr< Task > & item)
```

| Parámetro | Descripción |
| --- | --- |
| elemento | la tarea especificada que debe agregarse a esta colección de tareas. |

---

## Add (4 of 5) {#add_4}

Agrega una nueva tarea a la colección de tareas hijas.

**Returns:** returns the newly added instance of the Task class.

```cpp
Add(const System::String & taskName)
```

| Parámetro | Descripción |
| --- | --- |
| taskName | el nombre de la tarea especificada. |

---

## Add (5 of 5) {#add_5}

Agrega una nueva tarea recurrente a la colección de tareas hijas.

**Returns:** returns a task which was inserted before a task with the specified id.

```cpp
Add(const System::String & taskName, int32_t beforeTaskId)
```

| Parámetro | Descripción |
| --- | --- |
| taskName | el nombre de la tarea especificada. |
| beforeTaskId | El id especificado de una tarea antes del cual se insertará una nueva tarea. |

