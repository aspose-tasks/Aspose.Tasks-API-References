---
title: "Класс ProjectFileInfo"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.ProjectFileInfo. Экземпляр класса содержит информацию о формате файла проекта и версии Microsoft Project, в которой файл был создан"
type: docs
weight: 1460
url: /ru/net/aspose.tasks/projectfileinfo/
---
## ProjectFileInfo class

Экземпляр класса содержит информацию о формате файла проекта и версии Microsoft Project, в которой файл был создан.

```csharp
public sealed class ProjectFileInfo : IEquatable<ProjectFileInfo>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [CanRead](../../aspose.tasks/projectfileinfo/canread/) { get; } | Возвращает значение, указывающее, может ли Aspose.Tasks обрабатывать файл проекта. |
| [IsPasswordProtected](../../aspose.tasks/projectfileinfo/ispasswordprotected/) { get; } | Возвращает значение, указывающее, защищён ли проект паролем. |
| [ProjectApplicationInfo](../../aspose.tasks/projectfileinfo/projectapplicationinfo/) { get; } | Возвращает информацию о приложении файла проекта. |
| [ProjectFileFormat](../../aspose.tasks/projectfileinfo/projectfileformat/) { get; } | Возвращает формат файла проекта. |

## Методы

| Имя | Описание |
| --- | --- |
| override [Equals](../../aspose.tasks/projectfileinfo/equals/#equals_1)(object) | Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту. |
| [Equals](../../aspose.tasks/projectfileinfo/equals/#equals)(ProjectFileInfo) | Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту. |
| override [GetHashCode](../../aspose.tasks/projectfileinfo/gethashcode/)() | Возвращает значение хеш‑кода для экземпляра класса `ProjectFileInfo`. |

## Примечания

Используйте свойство CanRead, чтобы определить, что библиотека может обрабатывать файл проекта.

## Примеры

Показывает, как читать информацию о файле проекта.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


