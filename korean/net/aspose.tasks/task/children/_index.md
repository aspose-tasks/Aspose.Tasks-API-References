---
title: "Task.Children"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Task 속성. 이 객체의 하위 작업 컬렉션을 가져옵니다. 하위 작업을 나타내는 TaskCollection 객체입니다."
type: docs
weight: 190
url: /ko/net/aspose.tasks/task/children/
---
## Task.Children property

이 객체의 하위 작업 컬렉션을 가져옵니다. 하위 작업을 나타내는 TaskCollection 객체.

```csharp
public TaskCollection Children { get; }
```

## 예제

작업 컬렉션을 사용하여 작업을 추가하는 방법을 보여줍니다.

```csharp
var project = new Project();

// 작업, 하위 작업을 추가하고 프로젝트를 저장합니다.
var task = project.RootTask.Children.Add("Summary1");
task.Children.Add("Subtask1");
project.Save(OutDir + "CreateTasks_out.xml", SaveFileFormat.Xml);
```

### 또 보기

* class [TaskCollection](../../taskcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


