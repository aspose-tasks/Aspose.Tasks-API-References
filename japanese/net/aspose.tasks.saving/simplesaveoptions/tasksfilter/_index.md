---
title: "SimpleSaveOptions.TasksFilter"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "SimpleSaveOptions プロパティ。 ガント タスク シートおよびタスク使用チャートに描画されるタスクをフィルタリングするために使用される条件を取得または設定します"
type: docs
weight: 30
url: /ja/net/aspose.tasks.saving/simplesaveoptions/tasksfilter/
---
## SimpleSaveOptions.TasksFilter property

Gantt、タスクシート、タスク使用チャートに表示されるタスクをフィルタリングするために使用される条件を取得または設定します。

```csharp
public ICondition<Task> TasksFilter { get; set; }
```

## 備考

値が指定されていない場合、デフォルト フィルターが使用され、非表示タスク（つまり、折りたたまれたタスクの子タスク）が削除されます。

## 例

MS Project ファイルを保存する際にカスタム タスク フィルターを使用する方法を示します。

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

        // タスク フィルターを設定して、タスク 'Task5' と 'Task3' をスキップします
        TasksFilter = new CustomTasksFilter()
    };

    // 保存形式を確認しましょう
    Console.WriteLine("The save format: " + options.SaveFormat);

    // ...

    // プロジェクトを画像として保存する
    project.Save(OutDir + "WorkWithTasksFilter_out.png", options);
}

/// <summary>
/// PDF 形式で MS Project ファイルを保存する際に使用できるカスタム タスク フィルターの例（例）。
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

### 関連項目

* interface [ICondition&lt;T&gt;](../../../aspose.tasks.util/icondition-1/)
* class [Task](../../../aspose.tasks/task/)
* class [SimpleSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../simplesaveoptions/)
* assembly [Aspose.Tasks](../../../)


