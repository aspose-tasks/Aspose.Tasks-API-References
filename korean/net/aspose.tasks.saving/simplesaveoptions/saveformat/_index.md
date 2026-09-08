---
title: "SimpleSaveOptions.SaveFormat"
second_title: "Aspose.Tasks for .NET API 참조"
description: "SimpleSaveOptions 속성. 이 저장 옵션 개체가 사용될 경우 문서가 저장될 형식을 가져오거나 설정합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks.saving/simplesaveoptions/saveformat/
---
## SimpleSaveOptions.SaveFormat property

이 저장 옵션 개체가 사용될 경우 문서가 저장되는 형식을 가져오거나 설정합니다.

```csharp
public SaveFileFormat SaveFormat { get; }
```

## 예제

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

* enum [SaveFileFormat](../../savefileformat/)
* class [SimpleSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../simplesaveoptions/)
* assembly [Aspose.Tasks](../../../)


