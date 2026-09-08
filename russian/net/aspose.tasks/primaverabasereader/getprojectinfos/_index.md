---
title: "PrimaveraBaseReader.GetProjectInfos"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод PrimaveraBaseReader. Возвращает список объектов краткой информации о проектах"
type: docs
weight: 10
url: /ru/net/aspose.tasks/primaverabasereader/getprojectinfos/
---
## PrimaveraBaseReader.GetProjectInfos method

Возвращает список объектов с краткой информацией о проекте.

```csharp
public List<PrimaveraProjectInfo> GetProjectInfos()
```

## Примеры

Показывает, как просмотреть информацию о коротких проектах из файла Primavera XML.

```csharp
var reader = new PrimaveraXmlReader(DataDir + "MultiprojectWithExternal.xml");
var projectInfos = reader.GetProjectInfos();
foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - {2}", info.Uid, info.Name, info.ExportFlag);
}
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

Показывает, как получить краткую информацию о проектах из базы данных Primavera.

```csharp
var settings = new PrimaveraDbSettings(GetConnectionString(), 0);

var reader = new PrimaveraDbReader(settings);
var projectInfos = reader.GetProjectInfos();

foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - '{2}'", info.Uid, info.ShortName, info.Name);
}

var firstProject = reader.LoadProject(projectInfos[0].Uid);
Console.WriteLine(firstProject.Uid);
Console.WriteLine(firstProject.Name);
Console.WriteLine(firstProject.PrimaveraProperties.ShortName);
```

### См. также

* class [PrimaveraProjectInfo](../../../aspose.tasks.primavera/primaveraprojectinfo/)
* class [PrimaveraBaseReader](../)
* namespace [Aspose.Tasks](../../primaverabasereader/)
* assembly [Aspose.Tasks](../../../)


