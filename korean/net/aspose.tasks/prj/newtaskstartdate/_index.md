---
title: "Prj.NewTaskStartDate"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 새 작업에 대한 기본 시작 날짜 유형"
type: docs
weight: 580
url: /ko/net/aspose.tasks/prj/newtaskstartdate/
---
## Prj.NewTaskStartDate field

새 작업에 대한 기본 시작 날짜 유형.

```csharp
public static readonly Key<TaskStartDateType, PrjKey> NewTaskStartDate;
```

## 예제

새 작업에 대한 속성을 설정하는 방법을 보여줍니다.

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);

Console.WriteLine("New Task Start Date: " + project.Get(Prj.NewTaskStartDate));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskStartDateType](../../taskstartdatetype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


