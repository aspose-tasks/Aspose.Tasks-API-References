---
title: "Класс ProjectInfo"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.ProjectInfo. Краткая информация о опубликованном проекте, доступном в Project Online"
type: docs
weight: 1470
url: /ru/net/aspose.tasks/projectinfo/
---
## ProjectInfo class

Краткая информация о опубликованном проекте, доступном в Project Online.

```csharp
public sealed class ProjectInfo
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [ProjectInfo](projectinfo/)() | Инициализирует новый экземпляр класса `ProjectInfo`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [CreatedDate](../../aspose.tasks/projectinfo/createddate/) { get; } | Получает дату и время создания проекта. |
| [Description](../../aspose.tasks/projectinfo/description/) { get; } | Получает описание проекта. |
| [Id](../../aspose.tasks/projectinfo/id/) { get; } | Получает уникальный идентификатор проекта. |
| [IsCheckedOut](../../aspose.tasks/projectinfo/ischeckedout/) { get; } | Получает значение, указывающее, заблокирован ли проект. |
| [LastPublishedDate](../../aspose.tasks/projectinfo/lastpublisheddate/) { get; } | Получает самую последнюю дату публикации проекта. |
| [LastSavedDate](../../aspose.tasks/projectinfo/lastsaveddate/) { get; } | Получает самую последнюю дату сохранения проекта. |
| [Name](../../aspose.tasks/projectinfo/name/) { get; } | Получает название проекта. |

## Примеры

Показывает, как читать информацию о проектах из Project Online.

```csharp
const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
const string UserName = "admin@contoso.onmicrosoft.com";
const string Password = "MyPassword";

var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);

var reader = new ProjectServerManager(credentials);
IEnumerable<ProjectInfo> list = reader.GetProjectList();

// читать информацию о проекте
Console.WriteLine("Print information about projects:");
foreach (var info in list)
{
    Console.WriteLine("Id: " + info.Id);
    Console.WriteLine("Name: " + info.Name);
    Console.WriteLine("Description: " + info.Description);
    Console.WriteLine("Created Date: " + info.CreatedDate);
    Console.WriteLine("Last Saved Date: " + info.LastSavedDate);
    Console.WriteLine("Last Published Date: " + info.LastPublishedDate);
    Console.WriteLine("Is Checked Out: " + info.IsCheckedOut);
}
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


