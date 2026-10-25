---
title: "Tsk.SubprojectName"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 하위 프로젝트의 원본 위치"
type: docs
weight: 1070
url: /ko/net/aspose.tasks/tsk/subprojectname/
---
## Tsk.SubprojectName field

하위 프로젝트의 소스 위치.

```csharp
public static readonly Key<string, TaskKey> SubprojectName;
```

## 예제

하위 프로젝트 작업을 만드는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "SubProjectTask.mpp");

// 작업 추가
var task = project.RootTask.Children.Add("Task 1");

// 새 하위 프로젝트 링크 설정
task.Set(Tsk.SubprojectName, DataDir + "subProject.mpp");

project.Save(OutDir + "CreateSubProjectTask_out.mpp", SaveFileFormat.Mpp);
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


