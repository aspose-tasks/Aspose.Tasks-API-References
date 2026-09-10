---
title: "ProjectServerManager"
second_title: "Справочник API Aspose.Tasks для Python через .NET"
description: 
type: docs
weight: 870
url: /ru/python-net/aspose.tasks/projectservermanager/
---

## ProjectServerManager class

Класс, который предоставляет методы для чтения и выполнения операций над проектами в указанной учётной записи Project Online или<br/>            в указанном локальном экземпляре Project Server (поддерживаются версии Project Server 2016 и 2019).

Тип ProjectServerManager раскрывает следующие члены:
## Конструкторы
| Имя | Описание |
| :- | :- |
| ProjectServerManager(credentials) | Инициализирует новый экземпляр класса [ProjectServerManager](/tasks/python-net/aspose.tasks/projectservermanager/). |
## Методы
| Имя | Описание |
| :- | :- |
| update_project(project) | Обновляет существующий проект в экземпляре Project Server\Project Online, используя параметры сохранения по умолчанию. Существующий проект будет перезаписан. |
| update_project(project, save_options) | Обновляет существующий проект в экземпляре Project Server\Project Online, используя указанные параметры сохранения. Существующий проект будет перезаписан. |
| create_new_project(project) | Создаёт новый проект в экземпляре Project Server\Project Online, используя параметры сохранения по умолчанию. |
| create_new_project(project, save_options) | Создаёт новый проект в экземпляре Project Server\Project Online, используя указанные параметры сохранения. |
| get_project(project_guid) | Получает проект с указанным GUID из учётной записи Project Online \ экземпляра Project Server. |
| get_project_raw_data(project_guid) | Получает двоичные данные проекта для целей устранения неполадок. |
| get_project_list() | Получает список проектов из хранилища 'Working' текущей учётной записи Project Online \ экземпляра Project Server. |

### См. также

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

