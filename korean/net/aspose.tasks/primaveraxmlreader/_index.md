---
title: "클래스 PrimaveraXmlReader"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.PrimaveraXmlReader 클래스. Primavera Xml 파일에서 프로젝트 UID를 검색할 수 있는 리더를 나타냅니다."
type: docs
weight: 1400
url: /ko/net/aspose.tasks/primaveraxmlreader/
---
## PrimaveraXmlReader class

Primavera Xml 파일에서 프로젝트 UID를 검색할 수 있는 리더를 나타냅니다.

```csharp
public class PrimaveraXmlReader : PrimaveraBaseReader
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [PrimaveraXmlReader](primaveraxmlreader/#constructor)(Stream) | `PrimaveraXmlReader` 클래스의 새 인스턴스를 초기화합니다. |
| [PrimaveraXmlReader](primaveraxmlreader/#constructor_1)(string) | `PrimaveraXmlReader` 클래스의 새 인스턴스를 초기화합니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [GetProjectInfos](../../aspose.tasks/primaverabasereader/getprojectinfos/)() | 프로젝트의 짧은 정보 객체 목록을 반환합니다. |
| [GetProjectUids](../../aspose.tasks/primaverabasereader/getprojectuids/)() | 프로젝트 고유 식별자 목록을 반환합니다. |
| virtual [LoadProject](../../aspose.tasks/primaverabasereader/loadproject/)(int) | 지정된 고유 식별자를 사용하여 프로젝트를 로드합니다. |

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

### 또 보기

* class [PrimaveraBaseReader](../primaverabasereader/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


