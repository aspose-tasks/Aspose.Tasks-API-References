---
title: "PrimaveraXmlSaveOptions.SkipSummaryAssignments"
second_title: "Aspose.Tasks for .NET API 참조"
description: "PrimaveraXmlSaveOptions 속성. 내보내기 중에 리소스를 요약 작업에 할당하는 작업을 건너뛸지 여부를 나타내는 값을 가져오거나 설정합니다."
type: docs
weight: 30
url: /ko/net/aspose.tasks.saving/primaveraxmlsaveoptions/skipsummaryassignments/
---
## PrimaveraXmlSaveOptions.SkipSummaryAssignments property

내보내기 중에 리소스를 요약 작업에 할당하는 것을 건너뛸지 여부를 나타내는 값을 가져오거나 설정합니다.

```csharp
public bool SkipSummaryAssignments { get; set; }
```

## 비고

Primavera 소프트웨어는 리소스를 요약(WBS) 작업에 할당하는 것을 지원하지 않습니다. 따라서 이러한 할당을 내보내면 Primavera 모델에 따라 잘못된 파일이 생성될 수 있습니다. true인 경우, 요약 작업에 대한 할당은 내보내기 중에 건너뛰어집니다. false(기본값)인 경우, 내보내기 중에 요약 작업에 대한 할당이 발견되면 예외가 발생합니다.

## 예제

SkipSummaryAssignments 플래그를 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var resource = project.Resources.Add("Resource");

var summaryTask = project.RootTask.Children.Add("Summary");
summaryTask.Children.Add("Task");

// Primavera는 리소스를 요약 작업에 할당하는 것을 지원하지 않습니다.
// 따라서 이러한 할당을 Primavera 형식으로 내보내면 Primavera에 가져올 수 없는 파일이 생성될 수 있습니다.
var assignment = project.ResourceAssignments.Add(summaryTask, resource);

var options = new PrimaveraXmlSaveOptions();
options.SkipSummaryAssignments = true;
project.Save(OutDir + "UseSkipSummaryAssignments_out.xml", options);
```

### 또 보기

* class [PrimaveraXmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../primaveraxmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


