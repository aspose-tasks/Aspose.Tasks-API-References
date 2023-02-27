---
title: ProjectServerManager.ProjectServerManager
second_title: Справочник по Aspose.Tasks для .NET API
description: ProjectServerManager строитель. Инициализирует новый экземплярProjectServerManager класс.
type: docs
weight: 10
url: /ru/net/aspose.tasks/projectservermanager/projectservermanager/
---
## ProjectServerManager constructor

Инициализирует новый экземпляр[`ProjectServerManager`](../) класс.

```csharp
public ProjectServerManager(ProjectServerCredentials credentials)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| credentials | ProjectServerCredentials | Учетные данные, используемые для подключения к учетной записи Project Online. |

### Примеры

В этом примере показано, как создать экземпляр ProjectServerManager для доступа к локальному экземпляру Project Server.

```csharp
[C#]
string site = "http://project_server_instance.local/";
var windowsCredentials = new NetworkCredential("Administrator", "my_password", "DOMAIN");
var projectServerCredentials = new ProjectServerCredentials(site, windowsCredentials);
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);
```

В этом примере показано, как создать экземпляр ProjectServerManager для доступа к учетной записи в службе Project Online.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "пароль");
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);
```

### Смотрите также

* class [ProjectServerCredentials](../../projectservercredentials/)
* class [ProjectServerManager](../)
* пространство имен [Aspose.Tasks](../../projectservermanager/)
* сборка [Aspose.Tasks](../../../)


