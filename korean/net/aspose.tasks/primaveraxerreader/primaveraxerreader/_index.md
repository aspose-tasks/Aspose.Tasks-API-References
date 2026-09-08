---
title: "PrimaveraXerReader.PrimaveraXerReader"
second_title: "Aspose.Tasks for .NET API 참조"
description: "PrimaveraXerReader 생성자. PrimaveraXerReader 클래스의 새 인스턴스를 초기화합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks/primaveraxerreader/primaveraxerreader/
---
## PrimaveraXerReader(string) {#constructor_1}

[`PrimaveraXerReader`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public PrimaveraXerReader(string xerFilePath)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| xerFilePath | 문자열 | .xer 파일 경로(Primavera 프로젝트가 위치한 곳). |

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

* class [PrimaveraXerReader](../)
* namespace [Aspose.Tasks](../../primaveraxerreader/)
* assembly [Aspose.Tasks](../../../)

---

## PrimaveraXerReader(Stream) {#constructor}

[`PrimaveraXerReader`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public PrimaveraXerReader(Stream stream)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 스트림 | 스트림 | Primavera XER 콘텐츠가 포함된 스트림. |

### 또 보기

* class [PrimaveraXerReader](../)
* namespace [Aspose.Tasks](../../primaveraxerreader/)
* assembly [Aspose.Tasks](../../../)


