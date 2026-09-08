---
title: "TasksFilter"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Gantt Task Sheet 및 Task Usage 차트에 렌더링된 작업을 필터링하는 데 사용되는 조건을 가져오거나 설정합니다."
type: docs
weight: 190
url: /ko/net/aspose.tasks.saving/saveoptions/tasksfilter/
---
## SaveOptions.TasksFilter property

간트, 작업 시트 및 작업 사용 차트에 렌더링된 작업을 필터링하는 데 사용되는 조건을 가져오거나 설정합니다.

```csharp
public ICondition<Task> TasksFilter { get; set; }
```

### 비고

값이 지정되지 않으면 기본 필터가 사용되어 보이지 않는 작업(예: 축소된 작업의 하위 작업)을 제거합니다.

### 예제

MS Project 파일을 저장하는 동안 사용자 정의 작업 필터를 사용하는 방법을 보여줍니다.

```csharp
public void WorkWithTasksFilter()
{
    var project = new Project(DataDir + "CreateProject2.mpp");

    var options = new PdfSaveOptions
    {
        PresentationFormat = PresentationFormat.GanttChart,
        PageSize = PageSize.A3,
        StartDate = new DateTime(2010, 7, 1),
        EndDate = new DateTime(2010, 9, 1),

        // 작업 'Task5'와 'Task3'을 건너뛰도록 작업 필터를 설정합니다.
        TasksFilter = new CustomTasksFilter()
    };

    // 저장 형식을 확인해 봅시다.
    Console.WriteLine("The save format: " + options.SaveFormat);

    // ...

    // 프로젝트를 이미지로 저장합니다
    project.Save(OutDir + "WorkWithTasksFilter_out.png", options);
}

/// <summary>
/// 예를 들어 PDF 형식으로 MS Project 파일을 저장할 때 사용할 수 있는 사용자 정의 작업 필터 예시입니다.
/// </summary>
/// <inheritdoc />
private class CustomTasksFilter : ICondition<Task>
{
    public bool Check(Task el)
    {
        return el.Get(Tsk.Name) != "Task5" && el.Get(Tsk.Name) != "Task3";
    }
}
```

### 또 보기

* interface [ICondition&lt;T&gt;](../../../aspose.tasks.util/icondition-1)
* class [Task](../../../aspose.tasks/task)
* class [SaveOptions](../../saveoptions)
* namespace [Aspose.Tasks.Saving](../../saveoptions)
* assembly [Aspose.Tasks](../../../)

<!-- 편집 금지: xmldocmd에 의해 Aspose.Tasks.dll용으로 생성됨 -->
