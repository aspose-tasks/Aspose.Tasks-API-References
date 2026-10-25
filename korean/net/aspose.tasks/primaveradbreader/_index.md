---
title: "클래스 PrimaveraDbReader"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.PrimaveraDbReader 클래스. Primavera DB에서 프로젝트 정보를 읽는 리더를 나타냅니다."
type: docs
weight: 1350
url: /ko/net/aspose.tasks/primaveradbreader/
---
## PrimaveraDbReader class

Primavera DB에서 프로젝트 정보를 읽는 리더를 나타냅니다.

```csharp
public sealed class PrimaveraDbReader : PrimaveraBaseReader
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [PrimaveraDbReader](primaveradbreader/)(PrimaveraDbSettings) | [`PrimaveraXerReader`](../primaveraxerreader/) 클래스의 새 인스턴스를 초기화합니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [GetProjectInfos](../../aspose.tasks/primaverabasereader/getprojectinfos/)() | 프로젝트의 짧은 정보 객체 목록을 반환합니다. |
| [GetProjectUids](../../aspose.tasks/primaverabasereader/getprojectuids/)() | 프로젝트 고유 식별자 목록을 반환합니다. |
| override [LoadProject](../../aspose.tasks/primaveradbreader/loadproject/)(int) | 지정된 고유 식별자를 사용하여 프로젝트를 로드합니다. |

## 예제

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

* class [PrimaveraBaseReader](../primaverabasereader/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


