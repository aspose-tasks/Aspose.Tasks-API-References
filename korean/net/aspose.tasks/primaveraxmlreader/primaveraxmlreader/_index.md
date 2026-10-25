---
title: "PrimaveraXmlReader.PrimaveraXmlReader"
second_title: "Aspose.Tasks for .NET API 참조"
description: "PrimaveraXmlReader 생성자. PrimaveraXmlReader 클래스의 새 인스턴스를 초기화합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks/primaveraxmlreader/primaveraxmlreader/
---
## PrimaveraXmlReader(string) {#constructor_1}

[`PrimaveraXmlReader`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public PrimaveraXmlReader(string templatePath)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| templatePath | 문자열 | Primavera Xml 프로젝트가 위치한 템플릿 경로 |

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

* class [PrimaveraXmlReader](../)
* namespace [Aspose.Tasks](../../primaveraxmlreader/)
* assembly [Aspose.Tasks](../../../)

---

## PrimaveraXmlReader(Stream) {#constructor}

[`PrimaveraXmlReader`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public PrimaveraXmlReader(Stream stream)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 스트림 | 스트림 | Primavera Xml 내용을 포함하는 스트림. |

## 예제

Primavera XML 스트림에서 프로젝트를 가져오는 방법을 보여줍니다.

```csharp
using (var stream = new FileStream(DataDir + "primavera.xml", FileMode.Open))
{
    var reader = new PrimaveraXmlReader(stream);
    List<int> projectUids = reader.GetProjectUids();
    foreach (var projectUid in projectUids)
    {
        Console.WriteLine("Project UID: " + projectUid);
    }
}
```

### 또 보기

* class [PrimaveraXmlReader](../)
* namespace [Aspose.Tasks](../../primaveraxmlreader/)
* assembly [Aspose.Tasks](../../../)


