---
title: "클래스 PrimaveraSaveOptions"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Saving.PrimaveraSaveOptions 클래스. 프로젝트를 Primavera XER 형식으로 저장할 때 추가 옵션을 지정할 수 있습니다."
type: docs
weight: 2150
url: /ko/net/aspose.tasks.saving/primaverasaveoptions/
---
## PrimaveraSaveOptions class

프로젝트를 Primavera XER 형식으로 저장할 때 추가 옵션을 지정할 수 있습니다.

```csharp
public class PrimaveraSaveOptions : SimpleSaveOptions
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [PrimaveraSaveOptions](primaverasaveoptions/)() | `PrimaveraSaveOptions` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [ActivityIdIncrement](../../aspose.tasks.saving/primaverasaveoptions/activityidincrement/) { get; set; } | 활동 ID 재번호 매기기에 사용되는 증가값을 가져오거나 설정합니다. |
| [ActivityIdPrefix](../../aspose.tasks.saving/primaverasaveoptions/activityidprefix/) { get; set; } | 활동 ID 재번호 매기기에 사용되는 접두사를 가져오거나 설정합니다. |
| [ActivityIdSuffix](../../aspose.tasks.saving/primaverasaveoptions/activityidsuffix/) { get; set; } | 활동 ID 재번호 매기기에 사용되는 접미사를 가져오거나 설정합니다. |
| [RenumberActivityIds](../../aspose.tasks.saving/primaverasaveoptions/renumberactivityids/) { get; set; } | 활동 ID를 재번호 매겨야 하는지를 나타내는 값을 가져오거나 설정합니다. |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | 이 저장 옵션 개체가 사용될 경우 문서가 저장되는 형식을 가져오거나 설정합니다. |
| [SkipSummaryAssignments](../../aspose.tasks.saving/primaverasaveoptions/skipsummaryassignments/) { get; set; } | 내보내기 중에 리소스를 요약 작업에 할당하는 것을 건너뛸지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | 간트 차트 및 작업 시트 차트에서 작업을 정렬하기 위한 비교자를 가져오거나 설정합니다. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | 간트, 작업 시트 및 작업 사용 차트에 렌더링된 작업을 필터링하는 데 사용되는 조건을 가져오거나 설정합니다. |

## 예제

다음과 작업하는 방법을 보여줍니다: &lt;see cref="Aspose.Tasks.Saving.PrimaveraSaveOptions" /&gt;.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// Primavera 저장 옵션을 생성하고 조정합니다
var options = new PrimaveraSaveOptions
                  {
                      // 활동의 접두사와 접미사를 정의합니다
                      ActivityIdPrefix = "TEST",
                      ActivityIdSuffix = 10000,

                      // 활동 재번호 매기기를 제어합니다
                      ActivityIdIncrement = 5,
                      RenumberActivityIds = true
                  };

project.Save(OutDir + "WorkWithPrimaveraSaveOptions_out.xer", options);
```

### 또 보기

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


