---
title: "Prj.ShowProjectSummaryTask"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 전체 프로젝트에 대한 요약 정보를 Gantt 차트 보기 상단에 자체 요약 작업 막대로 단일 행에 표시할지 여부를 결정합니다"
type: docs
weight: 640
url: /ko/net/aspose.tasks/prj/showprojectsummarytask/
---
## Prj.ShowProjectSummaryTask field

전체 프로젝트에 대한 요약 정보를 단일 행에 표시하고, Gantt 차트 보기 상단에 자체 요약 작업 막대를 포함할지 여부를 결정합니다.

```csharp
public static readonly Key<bool, PrjKey> ShowProjectSummaryTask;
```

## 예제

Prj.ShowProjectSummaryTask 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

project.Set(Prj.ShowProjectSummaryTask, true);

Console.WriteLine("Show Project Summary Task: " + project.Get(Prj.ShowProjectSummaryTask));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


