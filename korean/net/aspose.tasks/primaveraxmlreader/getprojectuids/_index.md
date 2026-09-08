---
title: "GetProjectUids"
second_title: "Aspose.Tasks for .NET API 참조"
description: "프로젝트 고유 식별자 목록을 반환합니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks/primaveraxmlreader/getprojectuids/
---
## PrimaveraXmlReader.GetProjectUids method

프로젝트 고유 식별자 목록을 반환합니다.

```csharp
public List<int> GetProjectUids()
```

### 반환 값

프로젝트 고유 식별자 목록.

### 예제

Primavera XML 파일에서 프로젝트를 가져오는 방법을 보여줍니다.

```csharp
var reader = new PrimaveraXmlReader(DataDir + "primavera.xml");
List<int> projectUids = reader.GetProjectUids();
foreach (var projectUid in projectUids)
{
    Console.WriteLine("Project UID: " + projectUid);
}
```

### 또 보기

* class [PrimaveraXmlReader](../../primaveraxmlreader)
* namespace [Aspose.Tasks](../../primaveraxmlreader)
* assembly [Aspose.Tasks](../../../)

<!-- 편집 금지: xmldocmd에 의해 Aspose.Tasks.dll용으로 생성됨 -->
