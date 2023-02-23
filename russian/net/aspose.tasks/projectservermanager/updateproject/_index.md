---
title: ProjectServerManager.UpdateProject
second_title: Справочник по Aspose.Tasks для .NET API
description: ProjectServerManager метод. Обновляет существующий проект в экземпляре Project ServerProject Online используя параметры сохранения по умолчанию. Существующий проект будет перезаписан.
type: docs
weight: 70
url: /ru/net/aspose.tasks/projectservermanager/updateproject/
---
## UpdateProject(Project) {#updateproject}

Обновляет существующий проект в экземпляре Project Server\Project Online, используя параметры сохранения по умолчанию. Существующий проект будет перезаписан.

```csharp
public void UpdateProject(Project project)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| project | Project | Проект, который необходимо сохранить в экземпляре Project Server\Project Online. |

### Исключения

| исключение | условие |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | В случае ошибки связи или ошибки, возвращенной сервером. |

### Примечания

Свойство проекта "project.Get(Prj.Guid)" должно быть допустимым идентификатором проекта, который существует в учетной записи Project Server \ экземпляре Project Online.

### Примеры

В этом примере проект загружается из учетной записи Project Online, изменяется и сохраняется обратно в учетную запись Project Online.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "пароль");
ProjectServerManager manager = new ProjectServerManager(credentials);
var projectList = manager.GetProjectList();
var projectGuid = projectList.First().Id;
var project = manager.GetProject(projectGuid);
var task = project.RootTask.Children.Add("New task");
manager.UpdateProject(project);
```

### Смотрите также

* class [Project](../../project/)
* class [ProjectServerManager](../)
* пространство имен [Aspose.Tasks](../../projectservermanager/)
* сборка [Aspose.Tasks](../../../)

---

## UpdateProject(Project, ProjectServerSaveOptions) {#updateproject_1}

Обновляет существующий проект в экземпляре Project Server\Project Online, используя указанные параметры сохранения. Существующий проект будет перезаписан.

```csharp
public void UpdateProject(Project project, ProjectServerSaveOptions saveOptions)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| project | Project | Проект, который необходимо сохранить в экземпляре Project Server\Project Online. |
| saveOptions | ProjectServerSaveOptions | Случай[`ProjectServerSaveOptions`](../../projectserversaveoptions/) сорт. |

### Исключения

| исключение | условие |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | В случае ошибки связи или ошибки, возвращенной сервером. |

### Примечания

Для saveOptions.ProjectGuid следует указать идентификатор проекта, который существует в экземпляре Project Server\ Project Online.

### Примеры

В этом примере проект загружается из учетной записи Project Online, изменяется и сохраняется обратно в учетную запись Project Online.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "пароль");
ProjectServerManager manager = new ProjectServerManager(credentials);
var projectList = manager.GetProjectList();
var projectGuid = projectList.First().Id;
var project = manager.GetProject(projectGuid);
var task = project.RootTask.Children.Add("New task");
manager.UpdateProject(project, new ProjectServerSaveOptions
{
    ProjectGuid = projectGuid
});
```

### Смотрите также

* class [Project](../../project/)
* class [ProjectServerSaveOptions](../../projectserversaveoptions/)
* class [ProjectServerManager](../)
* пространство имен [Aspose.Tasks](../../projectservermanager/)
* сборка [Aspose.Tasks](../../../)


