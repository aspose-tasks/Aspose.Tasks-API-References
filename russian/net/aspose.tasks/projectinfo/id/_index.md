---
title: "ProjectInfo.Id"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство ProjectInfo. Возвращает уникальный идентификатор проекта"
type: docs
weight: 40
url: /ru/net/aspose.tasks/projectinfo/id/
---
## ProjectInfo.Id property

Получает уникальный идентификатор проекта.

```csharp
public Guid Id { get; }
```

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

* class [ProjectInfo](../)
* namespace [Aspose.Tasks](../../projectinfo/)
* assembly [Aspose.Tasks](../../../)


