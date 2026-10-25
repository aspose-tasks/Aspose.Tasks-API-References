---
title: "클래스 PrimaveraXmlSaveOptions"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Saving.PrimaveraXmlSaveOptions 클래스. 프로젝트를 Primavera XML 형식으로 저장할 때 추가 옵션을 지정할 수 있습니다"
type: docs
weight: 2160
url: /ko/net/aspose.tasks.saving/primaveraxmlsaveoptions/
---
## PrimaveraXmlSaveOptions class

프로젝트를 Primavera XML 형식으로 저장할 때 추가 옵션을 지정할 수 있습니다.

```csharp
public class PrimaveraXmlSaveOptions : SimpleSaveOptions
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [PrimaveraXmlSaveOptions](primaveraxmlsaveoptions/)() | 새 `PrimaveraXmlSaveOptions` 클래스 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | 이 저장 옵션 개체가 사용될 경우 문서가 저장되는 형식을 가져오거나 설정합니다. |
| [SaveRootTask](../../aspose.tasks.saving/primaveraxmlsaveoptions/saveroottask/) { get; set; } | 루트 작업을 저장할지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [SkipSummaryAssignments](../../aspose.tasks.saving/primaveraxmlsaveoptions/skipsummaryassignments/) { get; set; } | 내보내기 중에 리소스를 요약 작업에 할당하는 것을 건너뛸지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | 간트 차트 및 작업 시트 차트에서 작업을 정렬하기 위한 비교자를 가져오거나 설정합니다. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | 간트, 작업 시트 및 작업 사용 차트에 렌더링된 작업을 필터링하는 데 사용되는 조건을 가져오거나 설정합니다. |

## 예제

Primavera XML 파일로 내보내는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "project.xml");

var options = new PrimaveraXmlSaveOptions();
options.SaveRootTask = false;
project.Save(OutDir + "UsingPrimaveraXMLSaveOptions_out.xml", options);
```

### 또 보기

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


