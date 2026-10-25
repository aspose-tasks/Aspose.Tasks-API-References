---
title: "Prj.AutoAddNewResourcesAndTasks"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj field. 새 리소스 또는 작업이 리소스 또는 작업 풀에 자동으로 추가되는지 여부를 결정합니다"
type: docs
weight: 50
url: /ko/net/aspose.tasks/prj/autoaddnewresourcesandtasks/
---
## Prj.AutoAddNewResourcesAndTasks field

새 리소스 또는 작업이 리소스 또는 작업 풀에 자동으로 추가되는지 여부를 결정합니다.

```csharp
public static readonly Key<NullableBool, PrjKey> AutoAddNewResourcesAndTasks;
```

## 예제

Prj.AutoAddNewResourcesAndTasks 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

project.Set(Prj.AutoAddNewResourcesAndTasks, true);

Console.WriteLine("Auto Add New Resources And Tasks: " + project.Get(Prj.AutoAddNewResourcesAndTasks));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


