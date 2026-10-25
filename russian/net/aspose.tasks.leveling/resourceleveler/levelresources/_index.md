---
title: "ResourceLeveler.LevelResources"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод ResourceLeveler. Выравнивает задачи для указанных ресурсов, используя заданные параметры выравнивания."
type: docs
weight: 30
url: /ru/net/aspose.tasks.leveling/resourceleveler/levelresources/
---
## ResourceLeveler.LevelResources method

Уравнивает задачи для указанных ресурсов, используя заданные параметры уравнивания.

```csharp
public static LevelingResult LevelResources(Project project, LevelingOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| проект | Project | Проект, к которому применяется выравнивание ресурсов. |
| опции | LevelingOptions | Параметры, определяющие, как выравнивать ресурсы. |

### Возвращаемое значение

Объект, содержащий результаты выравнивания ресурсов.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | если параметр options равен null. |

## Примеры

Показывает, как уравнивать конкретный ресурс, настраивать параметры уравнивания и просматривать сообщения алгоритма уравнивания.

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");

var levelingOptions = new LevelingOptions();
levelingOptions.StartDate = new DateTime(2013, 3, 10);
levelingOptions.FinishDate = new DateTime(2013, 4, 30);
levelingOptions.Resources = new List<Resource> { project.Resources.GetById(7) };
levelingOptions.MessageLevel = MessageLevel.Information;
levelingOptions.MessageHandler = new LevelingMessageHandler();

ResourceLeveler.LevelResources(project, levelingOptions);
```

### См. также

* class [LevelingResult](../../levelingresult/)
* class [Project](../../../aspose.tasks/project/)
* class [LevelingOptions](../../levelingoptions/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)


