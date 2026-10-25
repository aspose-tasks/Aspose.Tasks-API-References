---
title: "PrimaveraSaveOptions.ActivityIdPrefix"
second_title: "Aspose.Tasks for .NET API 참조"
description: "PrimaveraSaveOptions 속성. 활동 ID를 다시 번호 매기기에 사용되는 접두사를 가져오거나 설정합니다."
type: docs
weight: 30
url: /ko/net/aspose.tasks.saving/primaverasaveoptions/activityidprefix/
---
## PrimaveraSaveOptions.ActivityIdPrefix property

활동 ID 재번호 매기기에 사용되는 접두사를 가져오거나 설정합니다.

```csharp
public string ActivityIdPrefix { get; set; }
```

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

* class [PrimaveraSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../primaverasaveoptions/)
* assembly [Aspose.Tasks](../../../)


