---
title: "TaskCollection"
second_title: "Referencia de API de Aspose.Tasks para Python vía .NET"
description: 
type: docs
weight: 1140
url: /es/python-net/aspose.tasks/taskcollection/
---

## TaskCollection class

Representa una colección de [Task](/tasks/python-net/aspose.tasks/task/) objetos.

El tipo TaskCollection expone los siguientes miembros:
## Propiedades
| Nombre | Descripción |
| :- | :- |
| parent_project | Obtiene el proyecto principal del objeto TaskCollection. |
## Métodos
| Nombre | Descripción |
| :- | :- |
| add() | Agrega la tarea especificada a la instancia de la clase [TaskCollection](/tasks/python-net/aspose.tasks/taskcollection/).<br/>            Si ParentProject.CalculationMode es None, el usuario debe invocar Project.Recalculate() después de usar este método (Reprogramará todas las tareas del proyecto (fechas de inicio/fin, establece fechas tempranas/tardías) y calculará los campos dependientes como holguras, campos de trabajo y costo, identificadores y niveles de esquema).<br/>            Si ParentProject.CalculationMode es Manual, el método calculará solo el id de la tarea, el nivel de esquema y los números de esquema automáticamente.<br/>            Si ParentProject.CalculationMode es Automatic, el método reprograma todas las tareas del proyecto automáticamente<br/>            (fechas de inicio/fin, establece fechas tempranas/tardías, calcula holguras, campos de trabajo y costo, recalcula los identificadores y niveles de esquema). |
| add(task_name) | Agrega una nueva tarea a la colección de tareas hijas. |
| add(task_name, before_task_id) |  |
| add(parameters) | Inserta una nueva tarea antes de una tarea con el id especificado y en el mismo nivel de esquema. |
| to_list() | Convierte el objeto TaskCollection en una lista de objetos [Task](/tasks/python-net/aspose.tasks/task/). |
| get_by_uid(uid) | Devuelve una tarea con el Uid especificado cuyo ancestro es la tarea principal de esta colección. |
| get_by_id(id) | Devuelve una tarea con el Id especificado cuyo ancestro es la tarea principal de esta colección. |

### Ver también

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

