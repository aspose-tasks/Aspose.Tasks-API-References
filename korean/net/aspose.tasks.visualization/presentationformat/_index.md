---
title: "열거형 PresentationFormat"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Visualization.PresentationFormat 열거형. 프레젠테이션 형식에 대한 열거형"
type: docs
weight: 3270
url: /ko/net/aspose.tasks.visualization/presentationformat/
---
## PresentationFormat enumeration

프레젠테이션 형식에 대한 열거형입니다.

```csharp
public enum PresentationFormat
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| GanttChart | `0` | 간트 차트 프레젠테이션 형식. |
| TaskUsage | `1` | 작업 사용량 프레젠테이션 형식. |
| ResourceUsage | `2` | 리소스 사용량 프레젠테이션 형식. |
| ResourceSheet | `3` | 리소스 시트 프레젠테이션 형식. |
| TaskSheet | `4` | 작업 시트 프레젠테이션 형식. |

## 예제

리소스 시트 뷰를 렌더링하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ResourceSheetView.mpp");

SaveOptions options = new PdfSaveOptions();

// 프레젠테이션 형식을 리소스 시트로 설정합니다
options.PresentationFormat = PresentationFormat.ResourceSheet;
project.Save(OutDir + "ResourceSheetView_out.pdf", options);
```

### 또 보기

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


