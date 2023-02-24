---
title: TaskCollection.Add
second_title: Referencia de Aspose.Tasks para la API de .NET
description: TaskCollection método. Agrega la tarea especificada a la instancia delTaskCollectionclass. Si ParentProject.CalculationMode es Ninguno el usuario debe invocar Project.Recalculate después de usar este método reprogramará todas las tareas del proyecto fechas de inicio/finalización establece fechas tempranas/tardías y calculará los campos dependientes como horas libres trabajo y campos de costos ID y niveles de esquema. Si ParentProject.CalculationMode es Manual el método calculará automáticamente solo el ID de tarea el nivel de esquema y los números de esquema. Si ParentProject.CalculationMode es Automático el método reprograma todas las tareas del proyecto automáticamente inicio/fin fechas establece fechas tempranas/tardías calcula slacks campos de trabajo y costo recalcula ids y niveles de esquema.
type: docs
weight: 50
url: /es/net/aspose.tasks/taskcollection/add/
---
## Add(Task) {#add_4}

Agrega la tarea especificada a la instancia del[`TaskCollection`](../)class. Si ParentProject.CalculationMode es Ninguno, el usuario debe invocar Project.Recalculate() después de usar este método (reprogramará todas las tareas del proyecto (fechas de inicio/finalización, establece fechas tempranas/tardías) y calculará los campos dependientes, como horas libres, trabajo y campos de costos, ID y niveles de esquema). Si ParentProject.CalculationMode es Manual, el método calculará automáticamente solo el ID de tarea, el nivel de esquema y los números de esquema. Si ParentProject.CalculationMode es Automático, el método reprograma todas las tareas del proyecto automáticamente (inicio/fin fechas, establece fechas tempranas/tardías, calcula slacks, campos de trabajo y costo, recalcula ids y niveles de esquema).

```csharp
public void Add(Task item)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| item | Task | la tarea especificada que debe agregarse a esta colección de tareas. |

### Ver también

* class [Task](../../task/)
* class [TaskCollection](../)
* espacio de nombres [Aspose.Tasks](../../taskcollection/)
* asamblea [Aspose.Tasks](../../../)

---

## Add() {#add}

Agrega una nueva tarea a la colección de tareas del proyecto en el mismo nivel de esquema de la última tarea.

```csharp
public Task Add()
```

### Valor_devuelto

devuelve la instancia recién agregada del[`Task`](../../task/) clase.

### Ver también

* class [Task](../../task/)
* class [TaskCollection](../)
* espacio de nombres [Aspose.Tasks](../../taskcollection/)
* asamblea [Aspose.Tasks](../../../)

---

## Add(string) {#add_2}

Agrega una nueva tarea a la colección de tareas secundarias.

```csharp
public Task Add(string taskName)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| taskName | String | el nombre de la tarea especificada. |

### Valor_devuelto

devuelve la instancia recién agregada del[`Task`](../../task/) clase.

### Ver también

* class [Task](../../task/)
* class [TaskCollection](../)
* espacio de nombres [Aspose.Tasks](../../taskcollection/)
* asamblea [Aspose.Tasks](../../../)

---

## Add(string, int) {#add_3}

Agrega una nueva tarea recurrente a la colección de tareas secundarias.

```csharp
public Task Add(string taskName, int beforeTaskId)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| taskName | String | el nombre de la tarea especificada. |
| beforeTaskId | Int32 | La identificación especificada de una tarea antes de la cual se insertará una nueva tarea. |

### Valor_devuelto

devuelve una tarea que se insertó antes de una tarea con la identificación especificada.

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentOutOfRangeException | ArgumentOutOfRangeException se lanza si la identificación especificada no es una identificación de tarea válida. |

### Ver también

* class [Task](../../task/)
* class [TaskCollection](../)
* espacio de nombres [Aspose.Tasks](../../taskcollection/)
* asamblea [Aspose.Tasks](../../../)

---

## Add(RecurringTaskParameters) {#add_1}

Inserta una nueva tarea antes de una tarea con la identificación especificada y en el mismo nivel de esquema.

```csharp
public Task Add(RecurringTaskParameters parameters)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| parameters | RecurringTaskParameters | Los parámetros los parámetros especificados para la creación de tareas recurrentes. |

### Valor_devuelto

devuelve la instancia recién agregada del[`Task`](../../task/) clase.

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | Lanzado si los parámetros especificados son nulos. |
| ArgumentException | Se lanza si los parámetros especificados no son válidos. |

### Ver también

* class [Task](../../task/)
* class [RecurringTaskParameters](../../recurringtaskparameters/)
* class [TaskCollection](../)
* espacio de nombres [Aspose.Tasks](../../taskcollection/)
* asamblea [Aspose.Tasks](../../../)


