---
title: Class ProjectServerManager
second_title: Справочник по Aspose.Tasks для .NET API
description: Aspose.Tasks.ProjectServerManager сорт. Класс который предоставляет методы для чтения и выполнения операций над проектами в указанной учетной записи Project Online или в указанном локальном экземпляре Project Server поддерживаются версии Project Server 2016 и 2019.
type: docs
weight: 1250
url: /ru/net/aspose.tasks/projectservermanager/
---
## ProjectServerManager class

Класс, который предоставляет методы для чтения и выполнения операций над проектами в указанной учетной записи Project Online или в указанном локальном экземпляре Project Server (поддерживаются версии Project Server 2016 и 2019).

```csharp
public sealed class ProjectServerManager
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [ProjectServerManager](projectservermanager/)(ProjectServerCredentials) | Инициализирует новый экземпляр`ProjectServerManager` класс. |

## Методы

| Имя | Описание |
| --- | --- |
| [CreateNewProject](../../aspose.tasks/projectservermanager/createnewproject/#createnewproject)(Project) | Создает новый проект в экземпляре Project Server\Project Online, используя параметры сохранения по умолчанию. |
| [CreateNewProject](../../aspose.tasks/projectservermanager/createnewproject/#createnewproject_1)(Project, ProjectServerSaveOptions) | Создает новый проект в экземпляре Project Server\Project Online, используя указанные параметры сохранения. |
| [GetProject](../../aspose.tasks/projectservermanager/getproject/)(Guid) | Получает проект с указанным GUID из учетной записи Project Online \ Project Server instance. |
| [GetProjectList](../../aspose.tasks/projectservermanager/getprojectlist/)() | Получает список проектов из «Рабочего» хранилища текущей учетной записи Project Online \ Project Server instance. |
| [GetProjectRawData](../../aspose.tasks/projectservermanager/getprojectrawdata/)(Guid) | Получает двоичные данные проекта для устранения неполадок. |
| [UpdateProject](../../aspose.tasks/projectservermanager/updateproject/#updateproject)(Project) | Обновляет существующий проект в экземпляре Project Server\Project Online, используя параметры сохранения по умолчанию. Существующий проект будет перезаписан. |
| [UpdateProject](../../aspose.tasks/projectservermanager/updateproject/#updateproject_1)(Project, ProjectServerSaveOptions) | Обновляет существующий проект в экземпляре Project Server\Project Online, используя указанные параметры сохранения. Существующий проект будет перезаписан. |

## События

| Имя | Описание |
| --- | --- |
| event [ExecutingWebRequest](../../aspose.tasks/projectservermanager/executingwebrequest/) | Событие, возникающее при отправке веб-запроса в веб-API Project Server. |

### Смотрите также

* пространство имен [Aspose.Tasks](../../aspose.tasks/)
* сборка [Aspose.Tasks](../../)


