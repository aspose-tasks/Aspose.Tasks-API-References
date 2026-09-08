---
title: "Tsk.ActualStart"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업이 실제로 시작된 날짜와 시간"
type: docs
weight: 80
url: /ko/net/aspose.tasks/tsk/actualstart/
---
## Tsk.ActualStart field

작업이 실제로 시작된 날짜와 시간.

```csharp
public static readonly Key<DateTime, TaskKey> ActualStart;
```

## 예제

프로젝트 날짜가 평가 모드에서 재설정되는 것을 보여줍니다.

```csharp
var project = new Project();

// 새 작업을 만들기
var task1 = project.RootTask.Children.Add("Task1");
task1.Set(Tsk.ActualStart, new DateTime(2000, 2, 10, 8, 0, 0));
task1.Set(Tsk.ActualFinish, new DateTime(2000, 2, 10, 17, 0, 0));

var task2 = project.RootTask.Children.Add("Task2");
task2.Set(Tsk.ActualStart, new DateTime(2000, 2, 10, 8, 0, 0));
task2.Set(Tsk.ActualFinish, new DateTime(2000, 2, 10, 17, 0, 0));

project.Save(OutDir + "EvaluationDateTimeLimitations_out.xml", SaveFileFormat.Xml);
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


