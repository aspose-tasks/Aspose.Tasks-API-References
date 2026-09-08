---
title: "Project.RootTask"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Project 속성. 작업 트리의 루트를 가져옵니다"
type: docs
weight: 800
url: /ko/net/aspose.tasks/project/roottask/
---
## Project.RootTask property

작업 트리의 루트를 가져옵니다.

```csharp
public Task RootTask { get; }
```

## 예제

루트 프로젝트 작업을 사용하여 프로젝트에 작업을 추가하는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.Start, new DateTime(2012, 8, 23, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(24, TimeUnitType.Hour));
task.Set(Tsk.ActualStart, new DateTime(2012, 8, 23, 8, 0, 0));

project.Save(OutDir + "AddNewTask_out.xml", SaveFileFormat.Xml);
```

### 또 보기

* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


