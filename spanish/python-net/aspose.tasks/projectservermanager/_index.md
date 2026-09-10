---
title: "ProjectServerManager"
second_title: "Referencia de API de Aspose.Tasks para Python vía .NET"
description: 
type: docs
weight: 870
url: /es/python-net/aspose.tasks/projectservermanager/
---

## ProjectServerManager class

La clase que proporciona los métodos para leer y realizar operaciones en proyectos en la cuenta especificada de Project Online o<br/>            en la instancia local especificada de Project Server (se admiten las versiones 2016 y 2019 de Project Server).

El tipo ProjectServerManager expone los siguientes miembros:
## Constructores
| Nombre | Descripción |
| :- | :- |
| ProjectServerManager(credentials) | Inicializa una nueva instancia de la clase [ProjectServerManager](/tasks/python-net/aspose.tasks/projectservermanager/). |
## Métodos
| Nombre | Descripción |
| :- | :- |
| update_project(project) | Actualiza el proyecto existente en la instancia de Project Server\Project Online usando las opciones de guardado predeterminadas. El proyecto existente será sobrescrito. |
| update_project(project, save_options) | Actualiza el proyecto existente en la instancia de Project Server\Project Online usando las opciones de guardado especificadas. El proyecto existente será sobrescrito. |
| create_new_project(project) | Crea un nuevo proyecto en la instancia de Project Server\Project Online usando las opciones de guardado predeterminadas. |
| create_new_project(project, save_options) | Crea un nuevo proyecto en la instancia de Project Server\Project Online usando las opciones de guardado especificadas. |
| get_project(project_guid) | Obtiene el proyecto con el GUID especificado de la cuenta de Project Online \ instancia de Project Server. |
| get_project_raw_data(project_guid) | Obtiene los datos binarios del proyecto con fines de solución de problemas. |
| get_project_list() | Obtiene la lista de proyectos del almacén 'Working' de la cuenta actual de Project Online \ instancia de Project Server. |

### Ver también

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

