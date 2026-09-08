---
title: "Task.SplitParts"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Task 속성. 작업의 구간을 나타내는 SplitPart 컬렉션을 가져옵니다."
type: docs
weight: 1110
url: /ko/net/aspose.tasks/task/splitparts/
---
## Task.SplitParts property

작업의 구간을 나타내는 SplitPart 컬렉션을 가져옵니다.

```csharp
public SplitPartCollection SplitParts { get; }
```

## 예제

작업의 분할 구간을 표시하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ViewSplitTasks.mpp");

// 작업에 접근 
var task = project.RootTask.Children.GetById(4);

// 작업의 분할 구간을 표시합니다.
var collection = task.SplitParts;
foreach (var splitPart in collection)
{
    Console.WriteLine("Start: " + splitPart.Start + "\nFinish: " + splitPart.Finish + "\n");
}
```

### 또 보기

* class [SplitPartCollection](../../splitpartcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


