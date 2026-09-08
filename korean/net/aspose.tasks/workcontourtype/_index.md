---
title: "WorkContourType 열거형"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.WorkContourType 열거형. 작업의 컨투어를 지정합니다."
type: docs
weight: 3610
url: /ko/net/aspose.tasks/workcontourtype/
---
## WorkContourType enumeration

작업의 윤곽을 지정합니다.

```csharp
public enum WorkContourType
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| Undefined | `-1` | 값이 원본 프로젝트 파일에 정의되지 않았습니다. |
| Flat | `0` | 평탄한 작업 컨투어. |
| BackLoaded | `1` | 뒤쪽에 로드된 작업 컨투어. |
| FrontLoaded | `2` | 앞쪽에 로드된 작업 컨투어. |
| DoublePeak | `3` | 이중 피크 작업 컨투어. |
| EarlyPeak | `4` | 조기 피크 작업 컨투어. |
| LatePeak | `5` | 늦은 피크 작업 컨투어. |
| Bell | `6` | 벨 형태 작업 컨투어. |
| Turtle | `7` | 거북이 형태 작업 컨투어. |
| Contoured | `8` | 사용자 정의 작업 컨투어. |

## 비고

XML로 내보내는 동안 Undefined 값은 결과 XML에서 제거됩니다.

## 예제

리소스 할당에 대한 다양한 시간 단계 데이터 컨투어를 설정하는 방법을 보여줍니다.

```csharp
var project = new Project();
project.Set(Prj.StartDate, new DateTime(2000, 1, 3, 8, 0, 0));
project.Set(Prj.FinishDate, new DateTime(2000, 1, 7, 17, 0, 0));

// 작업 추가
var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
task.Set(Tsk.Finish, new DateTime(2000, 1, 3, 17, 0, 0));

var resource = project.Resources.Add("Resource");

// 리소스 할당 추가
var resourceAssignment = project.ResourceAssignments.Add(task, resource);
resourceAssignment.Set(Asn.Start, new DateTime(2000, 1, 3, 8, 0, 0));
resourceAssignment.Set(Asn.Work, project.GetWork(8));
resourceAssignment.Set(Asn.Finish, new DateTime(2000, 1, 3, 17, 0, 0));

// 플랫 컨투어는 기본 컨투어입니다
Console.WriteLine("Flat contour");

var collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}

// 컨투어 변경
Console.WriteLine("Turtle contour");
resourceAssignment.Set(Asn.WorkContour, WorkContourType.Turtle);
collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}

// 컨투어 변경
Console.WriteLine("BackLoaded contour");
resourceAssignment.Set(Asn.WorkContour, WorkContourType.BackLoaded);
collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}

// 컨투어 변경
Console.WriteLine("FrontLoaded contour");
resourceAssignment.Set(Asn.WorkContour, WorkContourType.FrontLoaded);
collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}

// 컨투어 변경
Console.WriteLine("Bell contour");
resourceAssignment.Set(Asn.WorkContour, WorkContourType.Bell);
collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}

// 컨투어 변경
Console.WriteLine("EarlyPeak contour");
resourceAssignment.Set(Asn.WorkContour, WorkContourType.EarlyPeak);
collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}

// 컨투어 변경
Console.WriteLine("LatePeak contour");
resourceAssignment.Set(Asn.WorkContour, WorkContourType.LatePeak);
collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}

// 컨투어 변경
Console.WriteLine("DoublePeak contour");
resourceAssignment.Set(Asn.WorkContour, WorkContourType.DoublePeak);
collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


