---
title: "Enum TaskStartDateType"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.TaskStartDateType 열거형. 작업 시작 날짜 유형을 지정합니다"
type: docs
weight: 2450
url: /ko/net/aspose.tasks/taskstartdatetype/
---
## TaskStartDateType enumeration

작업 시작 날짜 유형을 지정합니다.

```csharp
public enum TaskStartDateType
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| Undefined | `-1` | 필드 값이 원본 프로젝트 파일에 정의되지 않았습니다. |
| ProjectStartDate | `0` | 프로젝트 시작 날짜 |
| CurrentDate | `1` | 현재 날짜 |

## 비고

XML로 내보내는 동안 Undefined 값은 결과 XML에서 제거됩니다.

## 예제

작업의 기본 시작 날짜를 'CurrentDate'로 설정하는 방법을 보여줍니다.

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);
project.Save(OutDir + "SetAttributesForNewTasks_out.xml", SaveFileFormat.Xml);
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


