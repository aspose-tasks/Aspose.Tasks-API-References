---
title: "PrimaveraBaseReader.GetProjectInfos"
second_title: "Aspose.Tasks for .NET API 참조"
description: "PrimaveraBaseReader 메서드. 프로젝트의 간략 정보 객체 목록을 반환합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks/primaverabasereader/getprojectinfos/
---
## PrimaveraBaseReader.GetProjectInfos method

프로젝트의 짧은 정보 객체 목록을 반환합니다.

```csharp
public List<PrimaveraProjectInfo> GetProjectInfos()
```

## 예제

Primavera XML 파일에서 짧은 프로젝트의 정보를 검사하는 방법을 보여줍니다.

```csharp
var reader = new PrimaveraXmlReader(DataDir + "MultiprojectWithExternal.xml");
var projectInfos = reader.GetProjectInfos();
foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - {2}", info.Uid, info.Name, info.ExportFlag);
}
```

Primavera XER 파일에서 짧은 프로젝트의 정보를 검사하는 방법을 보여줍니다.

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

Primavera 데이터베이스에서 프로젝트의 간략 정보를 가져오는 방법을 보여줍니다.

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

### 또 보기

* class [PrimaveraProjectInfo](../../../aspose.tasks.primavera/primaveraprojectinfo/)
* class [PrimaveraBaseReader](../)
* namespace [Aspose.Tasks](../../primaverabasereader/)
* assembly [Aspose.Tasks](../../../)


