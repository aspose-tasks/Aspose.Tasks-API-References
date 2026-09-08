---
title: "클래스 PrimaveraXerReader"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.PrimaveraXerReader 클래스. Primavera XER 파일에서 프로젝트 UID를 읽는 리더를 나타냅니다."
type: docs
weight: 1390
url: /ko/net/aspose.tasks/primaveraxerreader/
---
## PrimaveraXerReader class

Primavera XER 파일에서 프로젝트 UID를 읽는 리더를 나타냅니다.

```csharp
public sealed class PrimaveraXerReader : PrimaveraBaseReader
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [PrimaveraXerReader](primaveraxerreader/#constructor)(Stream) | `PrimaveraXerReader` 클래스의 새 인스턴스를 초기화합니다. |
| [PrimaveraXerReader](primaveraxerreader/#constructor_1)(string) | `PrimaveraXerReader` 클래스의 새 인스턴스를 초기화합니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [GetProjectInfos](../../aspose.tasks/primaverabasereader/getprojectinfos/)() | 프로젝트의 짧은 정보 객체 목록을 반환합니다. |
| [GetProjectUids](../../aspose.tasks/primaverabasereader/getprojectuids/)() | 프로젝트 고유 식별자 목록을 반환합니다. |
| virtual [LoadProject](../../aspose.tasks/primaverabasereader/loadproject/)(int) | 지정된 고유 식별자를 사용하여 프로젝트를 로드합니다. |

## 예제

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

* class [PrimaveraBaseReader](../primaverabasereader/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


