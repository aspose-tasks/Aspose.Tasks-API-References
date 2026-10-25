---
title: "PrimaveraBaseReader.LoadProject"
second_title: "Aspose.Tasks for .NET API 참조"
description: "PrimaveraBaseReader 메서드. 지정된 고유 식별자를 가진 프로젝트를 로드합니다."
type: docs
weight: 30
url: /ko/net/aspose.tasks/primaverabasereader/loadproject/
---
## PrimaveraBaseReader.LoadProject method

지정된 고유 식별자를 사용하여 프로젝트를 로드합니다.

```csharp
public virtual Project LoadProject(int projectUid)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| projectUid | Int32 | 로드할 프로젝트의 고유 식별자. |

### 반환 값

지정된 다중 프로젝트 파일에서 지정된 고유 식별자를 가진 프로젝트. 프로젝트가 존재하지 않으면 null.

## 예제

프로젝트 UID가 알려진 경우 Primavera XML 파일에서 프로젝트를 로드하는 방법을 보여줍니다.

```csharp
var reader = new PrimaveraXmlReader(DataDir + "PrimaveraProject.xml");
var project = reader.LoadProject(3882);
Console.WriteLine(project.Name);
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

### 또 보기

* class [Project](../../project/)
* class [PrimaveraBaseReader](../)
* namespace [Aspose.Tasks](../../primaverabasereader/)
* assembly [Aspose.Tasks](../../../)


