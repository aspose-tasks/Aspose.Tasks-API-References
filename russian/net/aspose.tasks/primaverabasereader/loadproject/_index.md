---
title: "PrimaveraBaseReader.LoadProject"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод PrimaveraBaseReader. Загружает проект с указанным уникальным идентификатором"
type: docs
weight: 30
url: /ru/net/aspose.tasks/primaverabasereader/loadproject/
---
## PrimaveraBaseReader.LoadProject method

Загружает проект с указанным уникальным идентификатором.

```csharp
public virtual Project LoadProject(int projectUid)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| projectUid | Int32 | Уникальный идентификатор проекта для загрузки. |

### Возвращаемое значение

Проект с указанным уникальным идентификатором из указанного многопроектного файла. Null, если проект не существует.

## Примеры

Показывает, как загрузить проект из файла Primavera XML, когда известен UID проекта.

```csharp
var reader = new PrimaveraXmlReader(DataDir + "PrimaveraProject.xml");
var project = reader.LoadProject(3882);
Console.WriteLine(project.Name);
```

Показывает, как просмотреть информацию о кратких проектах из файла Primavera XER.

```csharp
var reader = new PrimaveraXerReader(DataDir + "MultiprojectWithExternal.xer");
var projectInfos = reader.GetProjectInfos();
foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - {2}", info.Uid, info.Name, info.ExportFlag);
}

var project = reader.LoadProject(5494);

Console.WriteLine("Loaded project '{0}' with Uid {1}", project.Name, project.Uid);
```

### См. также

* class [Project](../../project/)
* class [PrimaveraBaseReader](../)
* namespace [Aspose.Tasks](../../primaverabasereader/)
* assembly [Aspose.Tasks](../../../)


